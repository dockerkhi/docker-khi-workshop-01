# this same shows how we can extend/change an existing official image from Docker Hub

FROM httpd:alpine
# highly recommend you always pin versions for anything beyond dev/learn

WORKDIR /usr/local/apache2/htdocs/
# change working directory to root of apache
# using WORKDIR is prefered to using 'RUN cd /some/path'

COPY index.html index.html

# I don't have to specify EXPOSE or CMD because they're in my FROM
