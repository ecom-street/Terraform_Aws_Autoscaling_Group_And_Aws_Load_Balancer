# Terraform_Aws_Autoscaling_Group

AWS Auto Scaling groups (ASGs) let you easily scale and manage a collection of EC2 instances that run the same instance configuration. You can then manage the number of running instances manually or dynamically, allowing you to lower operating costs. Since ASGs are dynamic, Terraform does not manage the underlying instances directly because every scaling action would introduce state drift. You can use Terraform lifecycle arguments to avoid drift or accidental changes.

In this tutorial, you will use Terraform to provision and manage an Auto Scaling group and learn how Terraform configuration supports the dynamic aspects of the resource. You will launch an ASG with traffic managed by a load balancer and define a scaling policy to automatically modify the number of instances running in the group. You will learn how to use lifecycle arguments to avoid unwanted scaling of your ASG


