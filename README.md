https://engagedly.freshteam.com/jobs/ClkOybVRjER4/devops-engineer


import boto3
region ='region'
instances =['instance id' ]
ec2=boto3.client('ec2',region_name=region)

def lambda_handler(event,context):
    ec2.stop_instances(InstanceIds=instances)
    print('Stopped your instances:'+str(instances))
