sudo docker inspect -f "{{ .NetworkSettings.IPAddress }}" container_name
OR
docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' container_name
