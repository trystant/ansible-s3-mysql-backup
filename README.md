Backup to S3 using Ansible
=========================

Ansible task that makes a backup of a MySQL database and uploads it to
an AWS S3 bucket.  

## Getting Started

Clone the repository from the [repository](git@github.com:trystant/ansible-s3-mysql-backup.git)
Update the `vars.yml` file with the following credentials:
* deploy_user - SSH account
* db_name - Database username
* mysql_user - MyQL username
* mysql_password - MySQL password
* AWS Access Key - AWS Credentials
* AWS Secret Key - AWS Credentials


### Prerequisites
* AWS Account
* Single Host with SSH account in one host configuration
* Public key SSH connection between source & destination SSH accounts in
  two hose configuration
* Python 2.6+ installed, with the following modules:
  * pip
  * python-mysqldb
  * boto
  * boto3
  * botocore

### Installing

A step by step series of examples that tell you have to get a development env running

Clone the repo from [GitHub](https://github.com/trystant/ansible-s3-mysql-backup).

```
$ git clone git@github.com:trystant/ansible-s3-mysql-backup.git
```

Install Python 2.6+


## Running the Backup Task
```
ansible-playbook -i hosts backup.yml
```


End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system
