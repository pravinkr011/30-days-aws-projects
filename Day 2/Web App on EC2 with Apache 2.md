# EC2-based Web Server – Configure Apache/Nginx on an EC2 #
instance. 
In this project, we will deploy a web server using Amazon EC2. We will launch an EC2 instance, install either Apache2 and configure it to serve a basic 
website. 
Steps to Set Up an EC2-based Web Server 
## Step 1: Launch an EC2 Instance ##
1. Go to the AWS Management Console → EC2. 
2. Click Launch Instance. 
3. Configure the instance: 
○ Name: MyWebServer 
○ AMI: Choose Ubuntu 
○ Instance Type: t2.micro (Free Tier eligible) 
○ Key Pair: Create a new key pair or use an existing one. 
○ Security Group: Allow SSH (port 22) and HTTP (port 80). 
4. Click Launch. 

### Step 2: Connect to the EC2 Instance ###
Open a terminal and run: 
connect using SSH [ use putty or mobaxterm]
Step 3: Install Apache2
For Apache (httpd) 
Update the package repository: 
``` sudo apt update -y ```  # Ubuntu 

### Install Apache: ###
``` sudo apt install apache2 -y ```

Start and enable Apache: 
``` sudo systemctl start apache2 ``` # Ubuntu 
``` sudo systemctl enable apache2 ``` # Ubuntu 

### Verify installation: ###
``` sudo systemctl status apache2 ``` # Ubuntu 

## Step 3: Deploy a Web Page##
Edit the default index file: 
sudo echo "<h1>Welcome to My Web Server</h1>" > /var/www/html/index.html 

## Step 4: Access the Web Server ##
Open a browser and go to: 
http://your-instance-public-ip 
