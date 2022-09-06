# My Base Image
FROM ubuntu:16.04

# Owner & Maintainer of this Image. 
MAINTAINER Pawan Kawade <pawankawade@gmail.com>

# Initalized the APT Repo
RUN apt-get update 

# Install Apache Binary Pkg
RUN apt-get install -y apache2 

# Deploy Custom Index Page
COPY index.html /var/www/html/

# Bring the the Apache Application
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
