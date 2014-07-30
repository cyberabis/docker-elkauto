docker-elkauto
==============
Docker ELK container


Trying out this container
========================= 
Use “sudo” before commands if required.
Make sure docker is installed.
Run: docker pull cyberabis/docker-elkauto
Run: docker run -d -p 80:80 -p 3333:3333 -p 9200:9200 cyberabis/docker-elkauto /elk_start.sh
Launch Kibana at port 80 of your docker!


Sending data to ELK
===================
Logstash is listening in TCP port 3333. You can stream data like:
cat YOUR_FILE | nc DOCKER_IP 3333


Viewing data
============
Kibana runs at port 80. Just point your browser to your Docker IP.