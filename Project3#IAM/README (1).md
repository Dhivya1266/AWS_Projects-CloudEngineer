<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Cloud Security with AWS IAM

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-security-iam)

**Author:** dhivyapriya Pandiyaraj  
**Email:** dhivyapriya1999@gmail.com

---

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_1c864649)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate to create a IAM Policy, IAM User and groups and I'm doing this project to learn AWS

### Tools and concepts

Services I used were EC2, IAM Users, Groups and policy Key concepts I learnt include how to create start stop ec2 instance and how to create policy and how to create users and gropus and how to tag ec2 instaces and Account alias

### Project reflection

This project took me approximately 2 hous The most challenging part was applying permissions to the users. It was most rewarding to see when the iam policy has been created

---

## Tags

### What I did in this step

In this step, I will lanuch anEC2 Instance because to increase the computing power.

### Understanding tags

Tags are like lables used in the aws resources and when we need to apply policies and cost optimization it will easy filter and apply accordingly

### My tag configuration

The tag I’ve used on my EC2 instances is called ENV. The value I’ve assigned for my instances are Production and development

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_2e0e5a5d)

---

## IAM Policies

### What I did in this step

In this step, I will create an IAM policy because to restrict access to our intern from using the production environment and giving access to the Development environment

### Understanding IAM policies

IAM Policies are the rules to set the users , groups and services to which resources they have the access

### The policy I set up

For this project, I’ve set up a policy using JSON

### Policy effect

I’ve created a policy that allows users to start or stop the ec2 servives those are tagged under Env-Development

### Understanding Effect, Action, and Resource

The Effect, Action, and Resource attributes of a JSON policy means policy allowing the acctions

---

## My JSON Policy

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_1c864649)

---

## Account Alias

### What I did in this step

In this step, I will create account alias because to give an uniqe name instead of giving account ID

### Understanding account aliases

An account alias is a freindle name for ur account which displays in the url when u are sharing ur account

### Setting up my account alias

Creating an account alias took me less than minute Now, my new AWS console sign-in URL is https://dhivya-pl99.signin.aws.amazon.com/console

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_0eb4439b)

---

## IAM Users and User Groups

### What I did in this step

In this step, I will create users and groups because my intern should not have access to my own accont... So I need to create username and paswords for them

### Understanding user groups

IAM user groups are collections / folder of users which is used to give permissions as a set.

### Attaching policies to user groups

I attached the policy I created to this user group, which means the interns are capable to access my ec2 dev instance only

### Understanding IAM users

IAM users are the persons who can access your aws acount services

---

## Logging in as an IAM User

### Sharing sign-in details

The first way is .csv (Contaisn Ussers sign in url, Username, Password) and sending a mail with sign in details

### Observations from the IAM user dashboard

Once I logged in as my IAM user, I noticed that most of the services are not allowed  to view or edit.This was because i hav give access to only ENV-DEV EC2 Instance alone

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_6f2ab446)

---

## Testing IAM Policies

### What I did in this step

In this step, I will try to sign in with my IAM User intern1 cred because to check with they do not have the access to the Prod env ec2 instance

### Testing policy actions

I tested my JSON IAM policy by stopping the ec2 instances

### Stopping the production instance

When I tried to stop the production instance it throwed an error and  This was because the users are not having access to prod env

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_0e7a9d6a)

### Stopping the development instance

Next, when I tried to stop the development instance it stopped and This was because the users has the access to start or stop the env - dev tagged ec2 instance

![Image](http://learn.nextwork.org/lively_blue_brave_beaver/uploads/aws-security-iam_1811801c)

---

## IAM Policy Simulator

### Understanding the IAM Policy Simulator

### How I used the simulator

---

---
