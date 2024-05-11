```
sudo ufw status
sudo ufw enable
sudo ufw allow 8080/tcp
sudo ufw delete allow
sudo ufw disable

docker build -t image_name .
[OPTIONAL]docker build -t username/my_image:v1.0 .
docker build -t aiyaraaiya/easypdpa_web_api:v1.0.0 .

docker save -o easypdpa_web_api_v_1_0_0.tar aiyaraaiya/easypdpa_web_api:v1.0.0
docker load -i go_docker_test_v1.0.tar

sudo docker pull username/my_image:v1.0
sudo docker pull aiyaraaiya/go_docker_test:v1.0

sudo docker images

docker run -p -d host_port:container_port image_name
sudo docker run -d --name=demo-test -p 8079:8080 --network=bridge aiyaraaiya/go_docker_test:latest

sudo docker ps -a
sudo docker rm -f
curl 127.0.0.1:8079
```
