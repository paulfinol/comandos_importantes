sudo docker inspect -f "{{ .NetworkSettings.IPAddress }}" container_name
