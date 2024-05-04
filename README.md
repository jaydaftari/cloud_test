# cloud_test
1. creating a fast get and post api
2. creating docker file and deploying it to a render.com:
docker build -t myimage . 
docker run -d --name mycontainer -p 80:80 myimage
3. deploying it to aws ec2:
- can do it using putty
- can do it using cmd
- can do it using mobaxterm :
- click on session
- click on SSH
- insert public ipv4 address into remote host
- Enter your username for the EC2 instance (usually "ec2-user" for Amazon Linux or "ubuntu" for Ubuntu instances).
- put .pem file which you have downloaded while creating key value pair in use private key in advance SSH-browser type
- press OK
- Interact with Your EC2 Instance:
- Once connected, you'll have a terminal window where you can run commands on your EC2 instance as if you were using a local terminal.
- You can navigate the filesystem, install software, and perform other administrative tasks as needed.
- pwd #To see the current directory
- sudo su
-  yum update -y   # For Amazon Linux
- sudo apt update   # For Ubuntu
- sudo yum install docker # For Amazon Linux
-sudo apt install docker.io # For Ubuntu
- sudo usermod -a -G docker ec2-user  #Add the ec2-user (or your user) to the docker group to avoid using sudo every time you run 
4. Transfer required files in remote server, for mobxtream you can upload it using given right icons.
5. Docker commands: Insert same docker commands that we have used previously

# use ecr: 
