---
layout: post
title: "Install and configure the AWS CLI - macOS"
author: "Arne"
categories: journal
tags: [aws, cli, commandline, configure, configuration, terminal]
---

The AWS CLI is a command line interface, which enables you to create and interact with your AWS account
via the command line.

### Installation:

First, you can download the current version of the AWS CLI with the curl command.
```terminal
$ curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
```

Then you can install the AWS CLI with the standard macOS installation program.
```terminal
$ sudo installer -pkg ./AWSCLIV2.pkg -target /
```

Now, let´s check if the installation was successfull:
```terminal
$ which aws
```

Another way to test the installation:
```terminal
$ aws --version
```

### Configuration:

Before you can create or administrate your resoruces, you need to configure your AWS profile.
```terminal
$ aws configure
```

You are then prompted to enter details about your AWS account like your Access Key ID and your Secret Access Key, your default region to create resources in and our preferred ouput format (the default it JSON, but you can also change it to text).

Press enter and that´s it .

### Summary
Now you can finally build in AWS with the terminal! I hope you enjoyed this Cloudspresso Shot 😄

###### Links:
The official tutorial of AWS can be found under the following link:
https://docs.aws.amazon.com/de_de/cli/latest/userguide/install-cliv2-mac.html#cliv2-mac-install-confirm
