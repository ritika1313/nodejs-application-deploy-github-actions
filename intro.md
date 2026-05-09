In this we will learn how to make CI/CD pipline to deploy node.js application using docker on private VPS. and we will also learn how we will automate this using github action

suppose our js code is running on the local server, we want to deploy this code on the server. first we will access the SSh to the server, developer use github a hosted version control system, our server will pull all the code from the github then by the help of the docker run the code. The main problem is that all these steps are quite manuall and we need to repeat it every time. This is where our CI/CD comes into the picture so we can actrually write the script. Github Action -> instructions (YAML) 1. whenever there is a PUSH 2. SSH into my server  3. CD /home/app     4. git pull 5. docker compose up -d

yaml file ko hmre server ke bre me kuch nhi pta to usko ssh ka access dena pdega 

id_rsa = PRIVATE key
id_rsa.pub = PUBLIC key