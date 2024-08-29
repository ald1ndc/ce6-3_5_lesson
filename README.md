# ce6-3_5_lesson
AWS ECR 

Please note that we have utilize the following link while working on this activity:

git@github.com:chathra222/ecs-ci-cd.git

Also, please note to update for MacOS(arm64) Docker Settings under General to ensure that the following is checked

 **Use containerd for pulling and storing images**

```
# docker buildx build --platform=linux/amd64,linux/arm64 --tag aldin/simple1-node-app .
# docker images
# docker tag aldin/simple1-node-app:latest 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/aldin/simple1-node-app:latest
# docker push 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/aldin/simple1-node-app:latest

# docker tag 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/aldin/simple1-node-app:latest 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/aldin/simple1-node-app:1
# docker images
# docker push 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/aldin/simple1-node-app:1
# cd terraform/
# terraform plan
# terraform apply
# terraform destroy
```
