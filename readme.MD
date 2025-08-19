## Steps:-
1. creating one ec2-instance and installing the jenkins in that ec2-server 
2. Launching the jenkins with the public-ip of the ec2-instance created in step-1
3. Installing the jenkins plugins
4. clicking on New Item and creating the freestye project
5. adding the github url and executing the script
6. creating the another ec2-instance for the agent and installing the required dependencies and libraries inside the agent server
7. configuring this agent in manage jenkins --> nodes --> Add new node and add the credentials of the ec2-server like username:ec2-user,password:DevOps321, Host:<PrivateIp-of-agent-server>, path: it can be anything like /home/ec2-user/<anyfilename>