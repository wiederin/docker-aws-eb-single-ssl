# docker-aws-eb-single-ssl
Template for a docker container to be deployed on an AWS Elastic Beanstalk Single Instance with https configured

## usage

### setup
1. Modify the Dockerfile to build required image or pull image from container registry
2. Modify the SSL certificates in .ebextensions/https-instance.config

### deploy
1. Commit latest changes & zip directory including .ebextensions and .platform directories (`git archive -o ../eb.zip HEAD`)

## todo
1. setup.sh to config certificates
2. setup.sh to specify image to pull
3. setup.sh to specify Dockerfile from Template
4. build with compose
5. ci pipeline (build image + deploy to server)
