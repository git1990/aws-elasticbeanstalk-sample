# aws-elasticbeanstalk-sample
Sample application written in node.js for demo purposes related to deploying to AWS Elastic Beanstalk

## Clone node application

1. git clone `git@github.com:wsieroci/aws-elasticbeanstalk-sample.git`
2. `cd` into it

## Pushing image to Docker Hub

1. docker images
2. docker tag fb2547b19d23 wsieroci/sample-postgres-node:latest
3. docker login
4. docker push wsieroci/sample-postgres-node:latest

## Create AIM user

1. Choosing name: wiktorsierocinski-demo
2. Copying Access Key, Secret Key and Password
3. Passing them to user

## Install aws eb cli

1. Maybe install the newest version: `pip install -U pip setuptools`
2. Or maybe install python: `curl https://bootstrap.pypa.io/ez_setup.py -o - | sudo python`
3. And then install pip: `sudo easy_install pip`
4. pip install awsebcli

## Init of eb cli

1. `eb init` - provide `aws-access-id` and `aws-secret-key`
2. Choose application name: `wiktorsierocinski-aws-sample`
3. Choose North Virginia as a region
4. `.elasticbeanstalk` directory will be created in your program root directory

## Create sample environment using aws sample application

1. `eb create --sample --vpc`
2. Provide vpc id (default one): `vpc-1c032a78`
3. EC2 subnets: `subnet-1b79d143, subnet-da1687ac, subnet-da1687ac, subnet-71b2c74c`
4. Default vpc security group: `sg-6c14be14`

## Deploy application to environment

1. `eb deploy wiktorsierocinski-aws-sample-dev`

## Create RDS PostgreSQL database




