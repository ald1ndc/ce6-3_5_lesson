# ce6-3_5_lesson
AWS ECR 

Please note For MacOS Docker Settings under General ensure that the following is checked

Use containerd for pulling and storing images

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
