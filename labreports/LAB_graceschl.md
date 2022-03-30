# Lab Report: CD
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Grace Schlauder  
**GitHub Handle:** https://github.com/grace-schl/   
**Repository:** [My Forked Repository](https://github.com/grace-schl/cis411_lab4_CD)  
**Collaborators:** [Michael Mourelatos](https://github.com/MichaelMourelatos)  
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> ![CircleCi Success](/assets/Screen%20Shot%202022-03-24%20at%204.27.23%20PM.png)

- [x] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it):  
> URL: http://cis411lab4-graceschl.herokuapp.com/graphql  
> ![Successful Test on Deployed URl](/assets/Deployed%20App.png)  
  
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> A containerized version of an application is beneficial because it allows all of the members of a project to the application without having to download a bunch of other programs. The container then holds all of the dependencies needed to run the project.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Programs like CircleCI allow for the code to be tested for errors before deploying it. This way, if the code is not deployable, the program will tell us and the errors can be fixed.
3. Why would you use a container technology over a virtual machine(VM)?
> Virtual machines typically take a lot longer to set up than container technology because container technologies require a lot less resources. 
4. What are some alternatives to Docker for containerized deployments?
> [Podman](https://podman.io/), [LXD](https://linuxcontainers.org/lxd/introduction/), and [rkt](https://cloud.redhat.com/learn/topics/rkt)
