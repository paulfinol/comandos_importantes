* sudo docker inspect -f "{{ .NetworkSettings.IPAddress }}" container_name
* docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' container_name ./
* docker exec -it container /bin/bash
* sudo sed -i -e "s|mirrorlist=|#mirrorlist=|g" /etc/yum.repos.d/CentOS-*
* sudo sed -i -e "s|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g" /etc/yum.repos.d/CentOS-*
