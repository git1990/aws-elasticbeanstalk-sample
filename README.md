# aws-elasticbeanstalk-sample
Sample application written in node.js for demo purposes related to deploying to AWS Elastic Beanstalk

## Pushing image to Docker Hub

0. docker images
1. docker tag fb2547b19d23 wsieroci/sample-postgres-node:latest
2. docker login
3. docker push wsieroci/sample-postgres-node:latest
