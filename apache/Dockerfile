#############################################################
# Archivo Dockerfile para ejecutar contenedores en Memcached
# Basado en una imagen de Ubuntu
#############################################################

# Establece la imagen de base a utilizar para Ubuntu
FROM ubuntu:14.04

# Establece el autor (maintainer) del archivo (tu nombre - el autor del archivo)
MAINTAINER Benjamin Guerrero

# Actualización de la lista de fuentes del repositorio de aplicaciones por defecto
RUN apt-get update


#Lenguajes 
RUN apt-get install -y language-pack-en
ENV LANGUAGE en_US.UTF-8
ENV LANG en_US.UTF-8
ENV LC_ALL en_US.UTF-8

RUN locale-gen en_US.UTF-8
RUN dpkg-reconfigure locales

# Instalar Apache
RUN apt-get install -y apache2

# Instalar php 5
RUN apt-get install -y libapache2-mod-auth-mysql php5-mysql php5 libapache2-mod-php5 php5-mcrypt

# Puerto para exponer
EXPOSE 6280


