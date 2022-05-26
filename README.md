* sudo docker inspect -f "{{ .NetworkSettings.IPAddress }}" container_name
* docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' container_name ./
* docker exec -it container /bin/bash
