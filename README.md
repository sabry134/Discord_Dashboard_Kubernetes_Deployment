~ Made by Sabry


**__Run Front image__**

```
docker run -d -p 8080:80 sabrysuperman/discord_front:latest
```

**__Run Back image__**

```
docker run -d -p 3000:3000 sabrysuperman/discord-api:latest
```

**__Kubernetes Deployment__**


```
./deploy.sh
```


Please note that it will work as the deployment is functional but clicking on pages such as about or admin will not work because it is still linked to "localhost:8080", thus not the kubernetes ip nor the node port. The dashboard code will soon be public to make such changes manually.


**This warning only applies to kubernetes, if you just run docker with the mentioned ports above, it should work normally**