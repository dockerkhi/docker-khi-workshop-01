## Exercise 4 - Creating your own public image
==============================================

For this exercise you will need an account on hub.docker.com. Once you have created the account, you will need to log into the CLI using `docker login`. You can then push your new images into this account.

1. Pull the httpd (Apache) image `docker pull httpd:alpine`
2. Lets run the image `docker run -it --name my-httpd httpd:alpine bash`
3. Let change the text in the default html file: `vi /usr/local/apache2/htdocs/index.html`
4. Change the 'It works!' to your name.

hint: You can move into edit mode by pressing `i`

hint: You can get out of edit mode by pressing `esc`

hint: Once you have done editing, press `shift + ;`, `wq` and then enter to save and quit the file.

5. Exit the container using `exit` command
6. Check if your changes hold using `docker diff my-httpd`
7. Save your Docker hub username in a variable `export YOUR_USERNAME=<USERNAME>`
8. Commit these changes using `docker commit -m "updated default html text" my-httpd $YOUR_USERNAME/my-httpd`. Make sure to replace YOUR_USERNAME with the username on Docker Hub
9. Check your newly created image `docker image ls`
10. Push your repository using `docker push $YOUR_USERNAME/my-httpd`
11. Check your new push repo on hub.docker.com.
