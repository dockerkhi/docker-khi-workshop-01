## Exercise 2 - Running detached containers
================================

1. Check if any container is running `docker container ls`
2. Run a long running container `docker run -d alpine sh -c 'while true; do date; sleep 1; done'`
3. Check the container is running `docker container ls`
4. Check the processes running `docker container top <ID>`. You will get the <ID> from the container list command (first column)
5. Check the logs of your container `docker container logs <ID>`
6. Check the meta data for your container `docker container inspect <ID>`
7. Stop your container `docker container stop <ID>`
8. Check container is stopped `docker container ls`
9. Remove your container `docker container rm <ID>`
