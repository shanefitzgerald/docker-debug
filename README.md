# How to debug:

1. open in Visual Studio Code
2. select debugger
3. attach to process (make sure Docker Node.js is selected) wait for it to attach.
4. run 
```bash
docker ps
```
5. find the container with image name in this example `dockerwebapp`
6. find the port that it mapped to. example
```
0.0.0.0:55002->8080/tcp
```
7. drop a break point.  In this example put the break point on line 12 of server.js
8. curl the mapped port. In this example
```
curl -i localhost:55002
```

Hopefully it breaks :fingerscrossed:

