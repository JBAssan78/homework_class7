**Running a AWS Server**


This project provides a step-by-step guide to creating an Amazon EC2 (Elastic Compute Cloud) instance using the AWS Management Console. It walks you through each stage of the process so that anyone — even without prior AWS experience — can follow along and successfully launch their own virtual server in the cloud.

You’ll learn how to set up a web-server development environment on AWS, configure key settings, and understand the deliverables involved. The guide also includes troubleshooting tips for common issues, ensuring a smooth and repeatable experience when creating EC2 instances.

By the end, you’ll have a fully functional cloud-based virtual server ready for development and testing.

What You’ll Learn

How to navigate and use the AWS Management Console

How to create and configure an EC2 instance

How to connect to your server using SSH

How to deploy a basic web server 

How to monitor, manage, and terminate instances

**Step 1**

If this is your first time using AWS you must first create an account, verify your email by signing and then go to your AWS management console.

Sign into AWS management console, click on “sign into console”. This will bring you to your IAM user sign in page. Fill in your account ID, IAM username and password and press enter.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/0acd6bc1c5c973738d14912117ab29c1cc5a2e1b/Screenshot%20(954).png)

Second sign in option

You can also sign in using your root user email. On the AWS sign-in page, click the option “Sign in using root user email” — this will display two sign-in options: Root user and IAM user. Select the appropriate option for your account, click Next, and then enter your credentials to sign in.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/edb0e3e05b7438bdebfc794de2f9a2692e1e9ba6/Screenshot%20(953).png)

**Step 2**
 
With sign in completed you should be on the AWS console home page, to make sure you did
look for your credentials that should be on your upper right hand side.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/1e5bf7e9a757c4002ced9f32c2962fc1af0e219d/Screenshot%20(955).png)


**Step 3**

In the search box on your left hand side type in EC2 and pick (EC2 virtual servers in cloud).
From the EC2 page look at the bar menu on your left hand side, scroll down to Network & 
Security and click on security groups.

On the security group page , select “create security group” which you will see on your right hand side. Fill in the basic details (name, description). Select inbounds HTTP, Anywhere IPv4. 
Do the same operation for inbounds SSH, Anywhere ipv4

**DO NOT TOUCH OUTBOUND FOR ANY REASON WHAT SO EVER!!!**

Scroll down and click on “create security group” which should be on your right hand side. 
Once it’s done you will be directed to another screen confirming your security group has been set up.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/e5ff56f8353cfc360bdd7a95c81b4ea6b9f13e4b/Screenshot%20(948).png)

**Step 4**

Now we can set up our instance, in the menu bar on your left hand side find the “instances”
Then click on (instances) which should be the first word you see when you scroll down.

Click on “Launch instances” you will be directed to a set up screen, from here fill in the need information name and tag and key pair for login if you have one (the key pair is optional)

![image_alt](https://github.com/JBAssan78/homework_class7/blob/f3ae7fdd935e3d59b0558544509966dc71b28e09/Screenshot%20(949).png)

Scroll down to “Network Settings” and look for (firewall “security group”). Click on select existing security group, you will see the security group you made earlier as an option choose it and go to advanced details.

Click on “advanced detail” scroll all the way down to where it says user data. This is where you put your information that will appear once your instance is complete (exp code), Click the orange button to Launch instance to be re-directed to the next page for confirmation.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/fdcc52f68a5891ce1370b68d1949f2b322ff4d12/Screenshot%20(950).png)

**Step 5**
Now that you're all set up we can check a couple of things , you’ll be given an instance summary for the server that you've set up. It will be a series of numbers starting with I-XXXXXXXXXX. Look for where it says “Public DNS, here is where we will start the server.

![image_alt](https://github.com/JBAssan78/homework_class7/blob/d4155db74d44512a5b627139c845c82554dc7a5b/Screenshot%20(957).png)

Now all we have to do from here is copy the DNS into the web browser. Type into the HTTP:// and you will see your work is done.



