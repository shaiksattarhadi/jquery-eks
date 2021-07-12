aws ecr get-login-password --region ca-central-1 | sudo docker login --username AWS --password-stdin 774418219404.dkr.ecr.ca-central-1.amazonaws.com
sudo docker build -t 774418219404.dkr.ecr.ca-central-1.amazonaws.com/jquerymarriage:$BUILD_NUMBER .
sudo docker push 774418219404.dkr.ecr.ca-central-1.amazonaws.com/jquerymarriage:$BUILD_NUMBER 