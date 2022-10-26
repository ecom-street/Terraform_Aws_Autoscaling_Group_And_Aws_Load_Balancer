# Terraform_Aws_Autoscaling_Group_And_Aws_Load_Balancer

We are a preferred AWS consultant and offers the best cloud AWS consulting service. Our AWS-certified expert consultants conduct a thorough review and evaluation of your existing IT infrastructure and service interaction model to provide top-notch solutions.
<h3><a href="https://www.ecomstreet.com/aws-consulting-services-company/" target="_blank">Schedule your free consultation today!</a></h3> <br/>

As soon as you learn how to manage basic network infrastructure in AWS using Terraform (see “Terraform recipe – Managing AWS VPC – Creating Public Subnet” and “Terraform recipe – Managing AWS VPC – Creating Private Subnets”), you want to start creating auto-scalable infrastructures.

# Auto Scaling Groups

Usually, Auto Scaling Groups are used to control the number of instances executing the same task like rendering dynamic web pages for your website, decoding videos and images, or calculating machine learning models.

Auto Scaling Groups also allows you to dynamically control your server pool size – increase it when your web servers are processing more traffic or tasks than usual, or decrease it when it becomes quieter.

In any case, this feature allows you to save your budget and make your infrastructure more fault-tolerant significantly.

Let’s build a simple infrastructure, which consists of several web servers for serving website traffic. In the following article, we’ll add RDS DB to our infrastructure.

Our infrastructure will be the following:

<img width="521" alt="c1" src="https://user-images.githubusercontent.com/115148205/197935178-eae2d1f9-9cba-405f-947d-c925604c0199.PNG">

# Setting up VPC.
Let’s assemble it in a new main.tf file. First of all, let’s declare VPC, two Public Subnets, Internet Gateway and Route Table (we may take this example as a base):

<img width="862" alt="1" src="https://user-images.githubusercontent.com/115148205/197942198-00ecb773-1830-4f85-bbcd-6a532720527f.PNG">
<img width="826" alt="2" src="https://user-images.githubusercontent.com/115148205/197942308-c7728a52-8880-4d47-8c22-361e953e5595.PNG">
<img width="818" alt="3" src="https://user-images.githubusercontent.com/115148205/197942396-d37274be-76a0-4645-8c63-75dfce6f425d.PNG">
<img width="815" alt="4" src="https://user-images.githubusercontent.com/115148205/197942720-e96a5c57-4ae5-48a3-afe2-da2b661b03df.PNG">
<img width="812" alt="5" src="https://user-images.githubusercontent.com/115148205/197942862-f4dbb0b7-b968-4bbf-9bbe-22aec6101eb9.PNG">
<img width="819" alt="6" src="https://user-images.githubusercontent.com/115148205/197943050-216fbc98-297c-4c79-9ee1-ab325ab8471a.PNG">
<img width="816" alt="7" src="https://user-images.githubusercontent.com/115148205/197943169-929da651-bc5f-4c6c-a762-1651ba58852b.PNG">
<img width="821" alt="8" src="https://user-images.githubusercontent.com/115148205/197943277-1e6cc7da-b367-4d39-a39b-032c3e7c93c6.PNG">







