# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Your Name  
**GitHub Handle:** isaacparada  
**Repository:** Your Forked Repository  
**Collaborators:** 
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here:  
> Example: [http://cis411lab4isaac-app.herokuapp.com/graphql](http://cis411lab4isaac-app.herokuapp.com/graphql)
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> Example: ![Successful Build](../labreports/Screen%20Shot%202021-04-06%20at%209.34.00%20PM.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> It is beneficial becuase it provides a seamless running environment for everyone working on the project. People can run and test the code from theoretically anywhere.
1. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> CirceCI is still important because it allows us to check the code against the criteria that you have set up. It's more than just deployment, it's about the checks that verify the code is suitable for deployment.
1. Why would you use a container technology over a virtual machine(VM)?
> It's easier to set up, and doesn't require a whole operating system that uses a lot more resources than are needed. A container lets you test what you need in a pretty customized environment.  
1. What are some alternatives to Docker for containerized deployments?
> From what I found online, there is VirtualBox, Containerd, Vagrant, Cloud Foundry, rkt, .. among others.