# docker-aws-eb-single-ssl
Template for a docker container to be deployed on an AWS Elastic Beanstalk Single Instance with https configured

## usage

### setup
1. Modify the Dockerfile to build required image or pull image from container registry
2. Modify the SSL certificates in .ebextensions/https-instance.config

### deploy
1. Commit latest changes (`git add .` + `git commit -m "message"`)
2. Zip directory (`git archive -o ../eb.zip HEAD`)

## todo
1. setup.sh to config ssl certificates
2. setup.sh to specify image to pull
3. setup.sh to specify Dockerfile from Template
4. build with compose
