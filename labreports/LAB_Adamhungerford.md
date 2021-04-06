# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Adam Hungerford
**GitHub Handle:** [adamhungerford](https://github.com/adamhungerford)
**Repository:** https://github.com/adamhungerford/cis411_lab4_CD
**Collaborators:** [Robbie Dorsey](https://github.com/airgo32)
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here: https://cis411lab4-cd-adamhungerford.herokuapp.com/graphql
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
![Successful build.](../assets/successful_deploy.PNG)
![Successful mutation.](../assets/successful_mutation.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> If you want to send this application out or have it work on other software, you'll need a container.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Continuous integration ensures a working product gets published, and ensures only quality, finished products end up on Heroku.
3. Why would you use a container technology over a virtual machine(VM)?
> Containers are much more lightweight and require much less overhead.
4. What are some alternatives to Docker for containerized deployments?
> LXC, Kubernetes, and rkt are alternatives.