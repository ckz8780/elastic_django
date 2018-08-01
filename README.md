# Elastic Django!

A little app to demonstrate the basic process for launching a modern Django app on AWS Elastic Beanstalk.

### Output of creation for Reference:

```
(venv_elastic_django) D:\CFE_Project\venv_elastic_django\src>eb create elastic-django-env
Creating application version archive "app-4ce5-180801_140232".
Uploading elastic_django/app-4ce5-180801_140232.zip to S3. This may take a while.
Upload Complete.
Environment details for: elastic-django-env
  Application name: elastic_django
  Region: us-east-1
  Deployed Version: app-4ce5-180801_140232
  Environment ID: e-hqhwn5rady
  Platform: arn:aws:elasticbeanstalk:us-east-1::platform/Python 3.6 running on 64bit Amazon Linux/2.7.1
  Tier: WebServer-Standard-1.0
  CNAME: UNKNOWN
  Updated: 2018-08-01 18:02:36.327000+00:00
Printing Status:
2018-08-01 18:02:35    INFO    createEnvironment is starting.
2018-08-01 18:02:36    INFO    Using elasticbeanstalk-us-east-1-747609117327 as Amazon S3 storage bucket for environment data.
2018-08-01 18:02:58    INFO    Created security group named: sg-23d3d169
2018-08-01 18:02:58    INFO    Created load balancer named: awseb-e-h-AWSEBLoa-IV1AJRIJD8XZ
2018-08-01 18:03:14    INFO    Created security group named: awseb-e-hqhwn5rady-stack-AWSEBSecurityGroup-YA0OS87C73Z5
2018-08-01 18:03:14    INFO    Created Auto Scaling launch configuration named: awseb-e-hqhwn5rady-stack-AWSEBAutoScalingLaunchConfiguration-1QDWUY1QYA3
2018-08-01 18:04:19    INFO    Created Auto Scaling group named: awseb-e-hqhwn5rady-stack-AWSEBAutoScalingGroup-1O7TS79RRJ944
2018-08-01 18:04:19    INFO    Waiting for EC2 instances to launch. This may take a few minutes.
2018-08-01 18:04:34    INFO    Created Auto Scaling group policy named: arn:aws:autoscaling:us-east-1:747609117327:scalingPolicy:cd4dd330-a8fb-4bfd-ab68a6d7b6bda:autoScalingGroupName/awseb-e-hqhwn5rady-stack-AWSEBAutoScalingGroup-1O7TS79RRJ944:policyName/awseb-e-hqhwn5rady-stack-AWSEBAutoScalingScaleUpPy-1MGQ97YDJBWAY
2018-08-01 18:04:34    INFO    Created Auto Scaling group policy named: arn:aws:autoscaling:us-east-1:747609117327:scalingPolicy:fea5e05c-7852-4207-81956edf008b6:autoScalingGroupName/awseb-e-hqhwn5rady-stack-AWSEBAutoScalingGroup-1O7TS79RRJ944:policyName/awseb-e-hqhwn5rady-stack-AWSEBAutoScalingScaleDownicy-3LOZTQ9G457K
2018-08-01 18:04:34    INFO    Created CloudWatch alarm named: awseb-e-hqhwn5rady-stack-AWSEBCloudwatchAlarmLow-K5L309OK2KXZ
2018-08-01 18:04:34    INFO    Created CloudWatch alarm named: awseb-e-hqhwn5rady-stack-AWSEBCloudwatchAlarmHigh-92XIVJ9HTGIB
2018-08-01 18:06:10    INFO    Successfully launched environment: elastic-django-env

(venv_elastic_django) D:\CFE_Project\venv_elastic_django\src>eb status
Environment details for: elastic-django-env
  Application name: elastic_django
  Region: us-east-1
  Deployed Version: app-4ce5-180801_140232
  Environment ID: e-hqhwn5rady
  Platform: arn:aws:elasticbeanstalk:us-east-1::platform/Python 3.6 running on 64bit Amazon Linux/2.7.1
  Tier: WebServer-Standard-1.0
  CNAME: elastic-django-env.ekpriwmptf.us-east-1.elasticbeanstalk.com
  Updated: 2018-08-01 18:06:10.483000+00:00
  Status: Ready
  Health: Green
```