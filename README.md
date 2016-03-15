Basic vagrant + ansile aws ec2 provision
========================================



This is repository contains all you need to provision a basic EC2 VM at AWS.

## Initial requirements:
* ansible 2.0.0.2 or higher
* vagrant 1.6.5 or higher
* vagrant-aws plugin 

## AWS account set up:

Please set up your AWS account and export the following variables:
```
$ export AWS_ACCESS_KEY='????????????????????'                      
$ export AWS_SECRET_KEY='????????????????????????????????????????'
$ export AWS_PRIVATE_KEY_PATH='~/.ssh/vagrant.pem'
$ export AWS_DEFAULT_REGION='us-east-1'
$ export AWS_EC2_KEY_NAME='vagrant'
$ export AWS_SECURITY_GROUP_NAME='vagrant'
```

## Usage
Install the vagrant-aws plugin as shown below:

```
$ vagrant plugin install vagrant-aws
...
$ vagrant up --provider=aws
...
```

Thank you for trying this environment and be free to contribute :)
