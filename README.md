# www
docker-compose example with NodeBB Ghost WordPress Nginx Mongodb miniproxy
## Usage:
- find all http://mydomain.com replace with your domain
- find all my@gmail.com replace with your name@gmail.com
```
docker-compose up -d
docker-compose logs -f
```
stop remove all containers
```
docker rm $(docker ps -aq)
docker rm $(docker ps -aq)
```
##Note:
Be sure to create local directory as **volumes** mentioned  in ***docker-compose.yml*** file to persistent user data, Otherwise when container removed by **[docker-compose rm -f]** all the user data will be gone. which can leading the app failed to start.
