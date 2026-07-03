# catalogue

create ROBOSHOP ---> floder --> create ---> save
ROBOSHOP --> create pipeline 

here versions are changing so we need read the version from package.json file
for this we need to install one pluggin inside json (pipeline utility steps) --> pluggin

Depending installations 

we need login into agent and run the 
dnf module disable nodejs
dnf module enable nodejs:20 -y
dnf install nodejs -y

create a webhook ---> configure --> add --> github hook 

now we need to create docker image
docker build -t URL/catalogue:appVersion

now we need to push to ECR

AWS --> Amzon ECR --> private registry ---> repo --> create --> roboshop/catalogue --> mutable --> create
there is a instruction tab it will show all process
1. we need to login for this we need to crate credentails 
pluggin --> aws credentails 

manage jenkins ---> credenatils ---> kind --> aws credentails --> aws-auth(id)--> ssh-cre --> acess key and secreat key 
pluggin --> aws steps
this for api hitting 
