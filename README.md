# Deploy Application for NestJS_HelloWorld_app

## Flow of diagram for Deploy the NestJS HelloWorld sample application on EC2 manually
![Deploy the NestJS HelloWorld sample application on EC2 manually](https://github.com/VyankateshwarTaikar/NestJS_HelloWorld_app/assets/102132721/1044e40f-a965-421a-a9ef-054f55d84b27) 


## 🔗Fork this Repo link
👉 [https://github.com/Shubhamrahangdale/helloworld0nest-js]

# 🕜Requirement 
1.AWS account with ec2 t2.micro/t3.micro - (Ubuntu)

2.Github account

3.Gtrong connection network

## Steps For NestJS HelloWorld sample application on EC2 manually 

## setup & upgrade repository
    
 sudo apt update 

 Then install Node.js-->   sudo apt install nodejs

 Check that the install was successful by querying node for its version number:   node -v

 If the package in the repositories suits your needs, this is all you need to do to get set up with Node.js. In most cases, you’ll also want to also install npm, the Node.js package manager. You can do this by installing the npm package with apt:    ---> sudo apt install npm

Add 3000 as a port in inbound rule

so we  can see the sucessfully deployed the application  with the help of manual deployment 


# flow diagram for Implement CI/CD using GitHub Actions.

![Nestjs Github action Deployment cicd](https://github.com/VyankateshwarTaikar/NestJS_HelloWorld_app/assets/102132721/b7799f63-48b5-45d2-a857-33480d2ca986)

## GitHub Actions Workflow (Deploy.yml):

1. Trigger the workflow on push to the main branch.
2. Checkout the code.
3. Set up Node.js environment.
4. Install dependencies.
5. Build the application.
6. Decode and set up the SSH key.
7. Deploy to EC2.

# 🌟Explanation of Secrets 
1.SSH_PRIVATE_KEY_BASE64: Base64 encoded SSH private key.(that you got while you creating Ec2 instance )

2.EC2_HOST: The EC2 instance's public IP or hostname.

3.EC2_USER: The SSH user for the EC2 instance, typically ubuntu for Ubuntu AMIs.


# 🌠Trigger Workflow:
The workflow is triggered when there is a push to the main branch.

## Checkout Code:
Uses the actions/checkout@v2 action to clone the repository.

## Set Up Node.js:
Uses the actions/setup-node@v3 action to set up Node.js version 18.

## Install Dependencies:
Runs npm install to install the necessary Node.js dependencies.

## Build Next.js App:

Runs npm run build to build the Next.js application.

## Decode and Set Up SSH Key:

Decodes the SSH private key from the GitHub secret and adds it to the ssh-agent for authentication with the EC2 instance.

## Deploy to EC2:

Connects to the EC2 instance using SSH and runs the deployment commands.

# 👉 when you Update Deploy.yml that will automatically run the deployment 

![image](https://github.com/VyankateshwarTaikar/NestJS_HelloWorld_app/assets/102132721/c262c687-c8f5-494d-9f09-5f497a3c74f9)

![image](https://github.com/VyankateshwarTaikar/NestJS_HelloWorld_app/assets/102132721/22e73e7f-785e-4e38-94ac-b313faef7e73)


![image](https://github.com/VyankateshwarTaikar/NestJS_HelloWorld_app/assets/102132721/35fd8bf2-95aa-420f-bbad-81167cd47f4c)


