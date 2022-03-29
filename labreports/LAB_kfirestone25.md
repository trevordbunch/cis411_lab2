# Lab Report: Cloud Container
___
**Course:** CIS 411, Spring 2022 
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Kylie Firestone
**GitHub Handle:** kfirestone25
**Repository:** https://github.com/kfirestone25/cis411_lab4_CD/tree/purelab
___

# Required Content

- [X] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [X] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [X] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [X] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> Example: ![Successful Build](../ex/trevordbunch_lab2_02.png)
- [X] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it):  
> https://cis411lab4-kfirestone25.herokuapp.com/graphql
- [X] Answer the **4** questions below.
- [X] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Just because an application runs smoothly on a local machine does not mean it will run the exact same way once it is shipped into production for others to use. Issues could arise from differences in operating systems, libraries, versions, etc.) Containers allow developers to develop their application locally, but also push their application upstream to ensure that it will work in production. 
1. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Heroku and CircleCI work together seemlessly to automate the process of delivery workflow. When using CircleCI, pushing a commit to the master means it goes through a continous pipeline where ultiple tests are performed. The code will only be pushed to Heroku if it passes those tests. Therefore, CircleCI serves as a check to ensure that code is running/working properly before pushing to Heroku in order to avoid unneccessary and irreversible errors. 
3. Why would you use a container technology over a virtual machine(VM)?
> Container technology essentially packages together everything you need to run an application or microservice (including the code, dependencies, operating system, etc) into one place. Therefore, a container allows you to run an application basically anywhere. This is not the case for virtual machines which contain operating system images. Due to this fact, containers utilize less overhead (system resources) and increase portability and efficiency. 
1. What are some alternatives to Docker for containerized deployments?
> Podman
> OpenVZ
> Containerd
> RunC
> LXC (Linux Containers)