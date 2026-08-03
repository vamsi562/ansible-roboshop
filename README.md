# ansible-roboshop

Install ec2 instances using ansible playbooks

# Pre-requisities
- Install botocore
  ``` pip install boto3 botocore ```

module: **amazon.aws.ec2_instance**

# Commands
------------

``` 
ansible-playbook -i inventory.ini -e "instance=['mongodb','mysql','redis','rabbitmq','cart','catalogue','payment','shipping','user','frontend']"  ec2_route53.yaml 

```


``` 
ansible-playbook -i inventory.ini mongodb.yaml
ansible-playbook -i inventory.ini catalogue.yaml
ansible-playbook -i inventory.ini cart.yaml
ansible-playbook -i inventory.ini user.yaml
ansible-playbook -i inventory.ini payment.yaml
ansible-playbook -i inventory.ini shipping.yaml
ansible-playbook -i inventory.ini mysql.yaml
ansible-playbook -i inventory.ini redis.yaml
ansible-playbook -i inventory.ini rabbitmq.yaml
ansible-playbook -i inventory.ini frontend.yaml
```