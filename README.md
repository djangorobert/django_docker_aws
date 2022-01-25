# django-docker-aws
Technologies use:
================
1.)Django Web Framework
2.)Docker Container
3.)Nginx
4.)Gunicorn
5.)AWS EC2, ECR, Elastic IP, 
6.)Github


This App used Django for the Backend with a Nginx Web Server. Docker was Utilized due to its ability to make working with teams easier. The was Containerized and then used AWS Cloud Instance to launch the site.

This Project was built to Connect a Django Python Web App with Docker and added to AWS Amazon Web Services.
The Project was first built on a local machine(PC) then once finished it was added to Github so that it could then be accessed by AWS EC2 Instance(VM) Virtual machine. I then used SSH to log in from my local computer (PC) to the EC2 Instance(VM) to then first download Docker to that PC and all the dependencies. After that I then used Git clone <myrepo> in the linux command line to download the local project that was added to Github. With the project now cloned in the EC2 instance I was able to run my docker commands, docker-compose build, docker images, then went to AWS Elastic Container Registry to get authentication token for repo to be able to push or pull with that done I was able to docker-compose push. 

After those commands in AWS ECR Elastic Contiainer Registry confirmed that the docker images were now there available in AWS. Now I was able to enter a final command docker-compose up -d.
Then was able to verify if my Hello Django App was live I went here:http://ec2-3-128-38-45.us-east-2.compute.amazonaws.com:8000/

One thing to remember this is for Education purposes always hide your security key in django with packages like django-environ and put Debug=False. 
Take Care.
