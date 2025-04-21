Scenario:  setting up a basic web server on an EC2 instance and storing the website's static files in an S3 bucket.

Part 1: Setting up an EC2 Instance

1. Launch an EC2 Instance:

o Navigate to the EC2 service in the AWS Management Console.

o Launch a new instance.

o Choose an appropriate Amazon Machine Image (AMI) (e.g., Amazon Linux 2 or Ubuntu).

o Select an instance type (t3.micro).

o Configure instance details (keep defaults for now).

o Add storage (keep defaults).

o Add tags (optional).

o Configure security group:

§ Allow SSH access (port 22) from your IP address.

§ Allow HTTP access (port 80) from anywhere.

o Review and launch the instance.

o Create a new key pair or use an existing one, and download the .pem file.

o Screenshot: Include a screenshot of the EC2 instance dashboard showing the running instance.

 

2. Connect to your EC2 instance

o Screenshot: Include a screenshot of  terminal showing a successful SSH connection to the EC2 instance.

 

3. Install a web server:

o Update the package repositories.

o Install a web server (Nginx).

o Start the webserver.

o Screenshot: Include a screenshot of the terminal showing the successful installation and start of the web server.

 

4. Create a simple HTML file:

o Create an index.html file in the web server's document root directory.

o Add some basic HTML content to the file.

5. Test the web server:

o Open a web browser and enter the public IPv4 address or DNS name of your EC2 instance.

o Verify that the index.html file is displayed.

o Screenshot: Include a screenshot of  web browser showing the rendered index.html file.

 

 

Part 2: Creating an S3 Bucket and Storing the HTML File

1. Create an S3 bucket:

o Navigate to the S3 service in the AWS Management Console.

o Create a new bucket.

o Choose a globally unique bucket name.

o Choose an AWS Region.

o Configure bucket settings (keep defaults).

o Disable block all public access for this assignment.

o Acknowledge the public access warning.

o Screenshot: Include a screenshot of the S3 bucket creation page, showing the bucket name and public access settings.

2. Upload the index.html file to the S3 bucket:

o Navigate to your created bucket.

o Upload the index.html file from your local machine.

o Screenshot: Include a screenshot of the S3 bucket showing the uploaded index.html file.

3. Make the object publicly accessible:

o Make the uploaded index.html file public.

4. Access the HTML file from S3:

o Find the object URL of the uploaded index.html file.

o Open a web browser and enter the object URL.

o Verify that the HTML file is displayed.

o Screenshot: Include a screenshot of web browser showing the rendered index.html file from the S3 URL.

