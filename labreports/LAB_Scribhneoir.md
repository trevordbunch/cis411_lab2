# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Josiah McCracken 
**GitHub Handle:** [Scribhnoeir] (https://github.com/scribhneoir) 
**Repository:** [Repo](https://github.com/scribhneoir/cis411_lab4_CD) 
**Collaborators:** 
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here:  
> [https://cis411lab4-scribhneoir.herokuapp.com/graphql](https://cis411lab4-scribhneoir.herokuapp.com/graphql)
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> ![Successful Build](..\assets\circleci.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> It is benificial when working on multiple machines, ensuring that everyone has the same virtual setup
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> The pipeline allows for further testing and configuration before deployment. 
3. Why would you use a container technology over a virtual machine(VM)?
> Container technology is more lightweight as compared to virtualizing a whole computer, os, etc. A container only contains what is necessary to run the application.
1. What are some alternatives to Docker for containerized deployments?
> Containerd, LXC, OpenVZ