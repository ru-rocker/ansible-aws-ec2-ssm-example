# Overview
An example to provision EC2 instances in the private subnet using Ansible dynamic inventory and community AWS collections.

# Ansible Version
ansible 2.10.4
    config file = None
    configured module search path = ['/Users/ru-rocker/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
    ansible python module location = /usr/local/Cellar/ansible/2.10.4/libexec/lib/python3.9/site-packages/ansible
    executable location = /usr/local/bin/ansible
    python version = 3.9.1 (default, Dec 29 2020, 07:31:08) [Clang 11.0.0 (clang-1100.0.33.17)]

# Python Libraries
There are two libraries required for this example, `boto3` and `botocore`.

# AWS Community Collections
Get the collections from ansible galaxy.

     ansible-galaxy collection install community.aws

# Run-it
How to execute the playbook

      ansible-playbook -i dev_aws_ec2.yml site.yml --extra-vars "access_key_id=XXXXXX aws_secret_access_key=YYYYYY"
