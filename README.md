# docker-jenkins-master

Jenkins master image

nginx as proxy:

docker run -d --name swun9-jenkins-master  swun9/jenkins-master

docker run -d -p 80:80 -v /opt/nginx/sites-enabled:/etc/nginx/sites-enabled  --link swun9-jenkins-master:jenkins swun9/nginx
