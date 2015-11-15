##Nginx, Node.js and docker-compose playground

Run `docker-compose up`, then `open "$(docker-machine ip $(docker-machine active))"` and check how the host changes on the web page as nginx routes between two containers.

###NGINX

Run nginx container: 
`docker run --name my_nginx -P -d nginx`

Check that it's running:
`curl $(docker-machine ip $(docker-machine active)):32769`

