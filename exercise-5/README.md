## Exercise 5 - Playing with ports
===================================

1. Lets run an image on a specific port: `docker run -d -p 8080:80 httpd:alpine`
2. Open browser and go to url `http://localhost:8080`
3. You should see "It works!" - this is being served by Apache inside the container