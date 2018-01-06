## Exercise 6 - Playing with volumes
===================================

1. Lets run an image with a volume: `docker run -dit -p 8080:80 -v "$PWD":/usr/local/apache2/htdocs/ httpd:alpine`
2. Open browser and go to url `http://localhost:8080`
3. You should see the replaced HTML file
4. Stop the container
5. Edit the HTML file in this folder (change it to your name)
6. Run again using the command above
7. Check the browser to see the changes reflected