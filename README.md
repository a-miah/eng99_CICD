# CI/CD 

- CI CD is considered as the backbone of DevOps practices and automation.
- Faster software builds, customer satisfaction by deploying the app in time.
- Small code changes make fault isolation simpler and quicker.

## Docker

- Virtualization platform to containerise your app.
- Continuous Integration Efficiency with Docker enables you to build a container image and use that same image across every step of the deployment process. 
- A huge benefit of this is the ability to separate non-dependent steps and run them in parallel.
- Makes it easier to create, deploy and run applications by using containers.
- Containers allow developers to package up an application with everything it needs, such as libraries and dependencies, and ship it out as as one package.


## CI - Continuous Integration
- Developers merge/commit code to master branch multiple times a day, fully automated build and test process which gives feedback within few minutes. This avoids issues which usually happens when people wait for release day to merge their changes into the release branch.


## CD - Continuous Delivery and Deployment

### Continous Delivery
- Continuous Delivery is an extension of continuous integration to make sure that you can release new changes to your customers quickly in a sustainable way. This means that on top of having automated your testing, you also have automated your release process and you can deploy your application at any point of time by clicking on a button.
- In continuous Delivery the deployment is completed manually.

### Continuous Deployment
- Every change that passes all stages of your production pipeline is released to your customers, there is no human intervention, and only a failed test will prevent a new change to be deployed to production.

### CICD Workflow 

![Alt text](https://github.com/a-miah/eng99_CICD/blob/main/Images/CICD-workflow.JPG "CICD Workflow")

## CI/CD Pipeline
- The CI/CD pipeline is all about automation: Initiating code builds, automated testing, and automated deploying to the staging or production environments.
- If the output of any stage fails, the next stage will also fail.


# Jenkins
- Jenkins is an open-source automation server in which the central build and CI process take place, It is a Java-based program with packages for Windows, macOS, & Linux.

![Alt text](https://github.com/a-miah/eng99_CICD/blob/main/Images/jenkins-pipeline.JPG "Jenkins Pipeline")

Many benefits:
- Great range of plugins available
- Supports building
- Deploying
- Automating for software development projects
- Easy installations
- Simple and user-friendly interface
- Extensible with huge community-contributed plugin resource
- Easy environment configuration in user interface & supports distributed builds with master-slave architecture

## Working with Jenkins
1.	Create new job
2.	Name it – eng99_attaik
3.	Freestyle project
4.	Description 
5.	Tick discard old builds - (max 3)
6.	Build > execute shell > save > apply
7.	Under name > build now > runs tests
8.	From build history > console output
9.	To run consecutive tests automatically > Post build actions > build other projects 
10.	Enter name of other project to run 


![Alt text](https://github.com/a-miah/eng99_CICD/blob/main/Images/jenkins_diagram.JPG "Jenkins Diagram")