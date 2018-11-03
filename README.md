# Sleeper to start/stop EC2 instance
A small Python script using boto to start/stop instance on Amazon AWS 

## Setup

First, you need Python [Boto](https://github.com/boto/boto)

Boto is already installed in most Amazon EC2 AMIs, if you are running it elsewhere, just:

### Debian/Ubuntu

```bash
sudo apt-get install python-boto
```
### Mac OS X

```bash
sudo easy_install pip
sudo pip install boto
```

### Windows

Ensure that you have installed Python on your windows. 
steps to install boto as per below.
```bash
$ git clone git://github.com/boto/boto.git
$ cd boto
$ python setup.py install
```
### Code requirement to work properly
You need to change Access Key ID (line 7) and Secret Access Key (line 9) accordingly in order to run this program.
Also, you need to specify the region of that particular EC2.
##### Kindly make sure to apply policy "EC2 Full Acces" to that particular user on IAM.

## Usage:

Example :
##### Start Ec2 Instance
```bash
sleeper.py start i-1234567890
```
##### Stop Ec2 Instance
```bash
sleeper.py stop i-1234567890
```

