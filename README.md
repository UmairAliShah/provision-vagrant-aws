Basic vagrant + ansile aws ec2 provision
========================================


This is repository contains all you need to provision a basic EC2 VM at AWS.

### Required packages:
For first, install the following packages at your unix system:
* vagrant 1.6.5 or higher
* ansible 2.0.0.2 or higher

### Install the vagrant-aws plugin:
The vagrant-aws plugin can be installed executing the following:
```
$ vagrant plugin install vagrant-aws
```

### AWS account set up:
Please set up your AWS account and export the following variables:
```
$ export AWS_ACCESS_KEY='????????????????????'                      
$ export AWS_SECRET_KEY='????????????????????????????????????????'
$ export AWS_PRIVATE_KEY_PATH='~/.ssh/vagrant.pem'
$ export AWS_DEFAULT_REGION='us-east-1'
$ export AWS_EC2_KEY_NAME='vagrant'
$ export AWS_SECURITY_GROUP_NAME='vagrant'
```

### Usage
After set the configuration listed above, just try the following line:
```
$ vagrant up --provider=aws
```

Thank you for trying this environment and be free to contribute :)
