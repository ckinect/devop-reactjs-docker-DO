# DevOps Reactjs Docker Github Netlify Pipeline

## Description
Automates the deployment process by setting up continuous delivery pipelines in the repository.
In this use case we use React app as our code along with Docker to standardize the development & testing environment 
and Github Actions which performs code compilation when there "code checkin" to main branch.

At the time of writing, I am unable to link Github package to deploy onto Netlify. Instead the following approach is used 👉
Deployment to Netlify is done by authorizing Netlify to read Github repository. Any code change in github will automatically 
deploy to Netlify.

![DevOps](pipeline.JPG?raw=true "Devops")

## Prerequisites
#### A Github account
#### A Netlify account
#### Docker installed on local machine
#### Vscode with Docker Plugin

## Get The React App
#### Either download the Zip file or use git clone
#### Once download, type "docker build -t my-app:dev ." to create and tag docker image
#### To run docker, type "docker run -itd -p 80:80 --rm my-app:dev"

### To CheckIn, 👉 run the following
#### git add -A
#### git commit -m '<your message>'
#### git push origin main
  
## Github Action [Build With Docker] 
![Build](Build.JPG?raw=true "Build")


## Future Improvement
#### Add Backlog/Kanban workflow integration such Confluence or Ansana
#### Integration with DigitalOcean with Docker support
