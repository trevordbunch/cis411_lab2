# Lab Report: CD
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Julina Metz  
**GitHub Handle:** julinametz  
**Repository:** https://github.com/julinametz/cis411_lab4_CD  
___

# Required Content

- [X] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [X] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [X] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [X] Write the URL of your running Heroku app here:  
> Example: [https://cis411lab4-julinametz.herokuapp.com/graphql](https://cis411lab4-julinametz.herokuapp.com/graphql)
- [X] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> Example: ![Successful Build](../assets/deploy.png)
- [X] Answer the **4** questions below.
- [X] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> A containerized version of the application is beneficial because they will run the same in the container, regardless of your operating system. This makes collaboration between people with different operating systems easier. 
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> The CI solution allows automated tests to be run before the code is deployed to ensure it is functioning properly.
3. Why would you use a container technology over a virtual machine(VM)?
> A container technology uses much less system resources than a virtual machine because it doesn't require an operating system to be installed on it. 
4. What are some alternatives to Docker for containerized deployments?
> Some alternatives for Docker are: Kubernetes, Mesos, and LXD.