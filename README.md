# ansible-roboshop

Install ec2 instances using ansible playbooks

# Pre-requisities
- Install botocore
  ``` pip install boto3 botocore ```

module: **amazon.aws.ec2_instance**

# Commands
------------

``` ansible-playbook -i inventory.ini -e "instance=['mongob','mysql','redis','rabbitmq','cart','catalogue','payment','shipping','user','frontend']"  ec2_route53.yaml ```


``` ==ansible-playbook -i inventory.ini mongodb.yaml== ```