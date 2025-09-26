# EC2-based Web Server – Configure Apache2 on an EC2 #
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



### ✅ Correct Format for GitHub (with copy button)

````markdown
sudo apt update -y
````

### Install Apache:

```bash
sudo apt install apache2 -y
```

### Start and enable Apache:

```bash
sudo systemctl start apache2
sudo systemctl enable apache2
```

### Verify installation:

```
sudo systemctl status apache2
```

### Deploy a web page:

<h1>Welcome to My Web Server</h1> 
sudo tree /var/www/html/index.html

---

```
sudo apt update -y
````
