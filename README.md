# DevOps Reactjs Docker Github Netlify Pipeline

## Description
Automates the deployment process by setting up continuous delivery pipelines in the repository.
In this use case we use React app as our code along with Docker to standardize the development & testing environment 
and Github Actions which performs code compilation when there "code checkin" to main branch.

At the time of writing, I am unable to link Github package to deploy onto Netlify. Instead the following approach is used 👉
Deployment to Netlify is done by authorizing Netlify to read Github repository. Any code change in github will automatically 
deploy to Netlify.

![DevOps](Devops.png?raw=true "Devops")

## Prerequisites
#### A Github account
#### A Netlify account

## Get The React App
#### Either download the Zip file or use git clone

### To CheckIn, 👉 run the following
#### git add -A
#### git commit -m '<your message>'
#### git push origin main
  
## Github Action [Build With Docker] 
