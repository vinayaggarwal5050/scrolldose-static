# scrolldose-static
Static website for scrolldose

# Running Nginx in docker
sudo docker run -d --restart=always --name nginx-server -p 80:80 -p 443:443 -v /mnt/data-drive/nginx-conf:/etc/nginx/conf.d -v /mnt/data-drive/nginx-files:/usr/share/nginx/html nginx:latest

# giving permssion to agent node user
sudo usermod -aG docker $USER && newgrp docker

# giving ownership
sudo chown -R pc2:pc2 /mnt/data-drive
