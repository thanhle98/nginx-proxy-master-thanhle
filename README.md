# This is nginx-proxy-master Docker-compose configuration

This tutorial is written by Thanhle. Guarantee working until Sep 2021

```
`nginx-proxy-master` is create by J21
Author: https://github.com/jc21/nginx-proxy-manager
This is a great tool for server to manage proxy using nginx. It has nice UI and easy configuration. Thank you very much to the author J21!
```

## How to run:

1. You will need `docker` and `docker-compose` to run the project
2. Just git clone this project to your server
3. run this command
```
docker stack deploy -c docker-compopse.yml nginx-proxy-master
```


## take-note: 

- This using swarm configuraiton. So remember your network: can connect to other docker's container in the service. You can try `sh` into the server and do some `ping` to check the `container-name` and `container port`. Very important! 
- The default sql database `jc21/mariadb-aria:latest` image is not working at the time I am using. Therefore, I replace the image with another one call `yobasystems/alpine-mariadb` 
