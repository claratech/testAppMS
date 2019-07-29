#update all existing package : yum -y update
#Install platform -yum -y install httpd
#copy the code to document: /var/www/html
#set any env variable for backend LB: BACKENDLB
#Apache is runni on port 80
# use ADD to copy files in that path or COPY to copy folder itself for File it's all the same
# Add is  sophisciated command

FROM centos:7
MAINTAINER CP@GMAIL.COM
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
ENV BACKENDLB=test
# to set author use MAINTAINER
EXPOSE 80
CMD ["apachectl", "-D", "FOREGROUND"]
#Aq-ROLE-NAME6:~/environment $docker build -t claratech/testAppMS:1.o testapp/frontend/
#runtime field and don't define in Docker 
#fileAPP-ROLE-NAME