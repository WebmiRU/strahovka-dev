#Dev-среда разработки для компании "Страховка.ру"

##Подготовка к работе
0. Установить `docker` и `docker-compose`

```
sudo docker network create --driver bridge strahovka
```
4. 
```
sudo docker run -p 80:80 -p 443:443 --name=strahovka_nginx --network="strahovka" ewolf34/strahovka-nginx
```


[comment]: <> (sudo docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data --network="strahovka" portainer/portainer-ce)