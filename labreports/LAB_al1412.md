# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Adam Lenker  
**GitHub Handle:** al1412  
**Repository:** https://github.com/al1412/cis411_lab4_CD  
**Collaborators:** 
___

# Required Content

- [X] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [X] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [X] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [X] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> ![Successful Build](https://user-images.githubusercontent.com/97567307/159940711-6a754a69-9d52-4792-bbe1-3b9827f60617.png)

- [X] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it):  
> [http://cis411lab4-al1412.herokuapp.com/graphql](http://cis411lab4-al1412.herokuapp.com/graphql)  
> ![Successful test deployed on Heroku](https://user-images.githubusercontent.com/97567307/159948747-f362189b-cab2-4f64-aae5-a9a475a9ee44.png)
- [X] Answer the **4** questions below.
- [X] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Even though an application can be run locally already, a containerized version improves an application's efficiency by using all available resources and minimizes overhead (the amount of time and resources needed to complete a specific task). If a containerized version is properly configured, then it can take advantage of pretty much all available resources and deployment of an application can be done through a single command in a terminal.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Deploying and publishing an application with a CI solution such as CircleCI allows the process of updating the app to be automated, with updated code being pushed to Heroku automatically through a single line of code in the terminal. Additionally, a user can deploy the same code to different branches within Heroku, which is useful if they have applications with a similar function that have been saved on there.
3. Why would you use a container technology over a virtual machine(VM)?
> Containers provide a way to virtualize an operating system (OS) so that multiple workloads can run within a single OS instance, as opposed to a virtual machine (VM) which virtualizes hardware of an OS and limits the amount of workloads it can run. Additionally, a conatiner requires fewer IT resources to run and deploy, as their images are measured in megabytes (MB) instead of gigabytes (GB) like VMs, resulting in less space and RAM being used in its processes.
4. What are some alternatives to Docker for containerized deployments?
> Some alternatives to Docker for containerized deployments include LXC (for Linux), Hyper-V (for Windows), Podman (an open-source engine), and containerd (a container runtime command).

## Additional content
Heroku API token:   
Client:      none (arrow brackets removed here since it would make the text disappear when putting it on markdown)   
ID:          18e42df6-cf34-4dfe-8935-df0be0907832   
Description: CIS411 Lab token   
Scope:       global   
Token:       ccbeef36-07a5-4534-8f55-e8bc6cd043dd   
Updated at:  Tue Mar 22 2022 14:02:30 GMT-0400 (Eastern Daylight Time) (less than a minute ago)   
