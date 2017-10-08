# www
docker-compose example with NodeBB Ghost WordPress Nginx Mongodb
## Usage:
- find all http://mydomain.com replace with your domain
- find all my@gmail.com replace with your name@gmail.com
```
docker-compose up -d
docker-compose up logs -f
```
##Note:
Be sure to create local directory as **volumes** mentioned  in ***docker-compose.yml*** file to persistent user data, Otherwise when container removed by **[docker-compose rm -f]** all the user data will be gone. which can leading the app failed to start.
