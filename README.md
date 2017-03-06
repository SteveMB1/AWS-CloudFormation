# Amazon Web Services(AWS) CloudFormation
If you have any questions feel free to contact with me. I may take a day to respond but I will get back to you. If this helps you, please Star(⭐️) this reponitory. 😁 
## Auto Scaling Elastic Beanstalk
This was designed to be deployed inside us-east-1 datacenter. Instances are placed inside the private subnets, internet traffic coming from the load balancer traverses through the public subnets.
#### VPC: 10.1.0.0 - 10.1.15.255 /20

#### Public Subnets:
  * 1 /28 10.1.14.0 - 10.1.14.15
  * 2 /28 10.1.14.16 - 10.1.14.31
  * 3 /28 10.1.14.32 - 10.1.14.47
  
#### Private Subnets:
  * 1 /22 10.1.0.0 - 10.1.3.255
  * 2 /22 10.1.4.0 - 10.1.7.255
  * 3 /22 10.1.8.0 - 10.1.11.255
  * 4 /23  10.1.12.0 - 10.1.13.255

![Result](https://github.com/SteveMB1/AWS-CloudFormation/blob/master/ElasticBeanstalk-4Private-Subnets.png?raw=true)
Sources: 
http://docs.aws.amazon.com/cli/latest/reference/elasticbeanstalk/describe-configuration-options.html
http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/command-options.html#configuration-options-recommendedvalues
http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/vpc-rds.html
http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-beanstalk-configurationtemplate.html
