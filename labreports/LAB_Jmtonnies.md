# Lab Report: CD
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Joseph Tonnies  
**GitHub Handle:** Jmtonnies  
**Repository:** https://github.com/Jmtonnies/cis411_lab4_CD
**Collaborators:** alecclyde
___

# Required Content

- [✓] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [✓] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [✓] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [✓] Write the URL of your running Heroku app here: http://cis411lab4-jmtonnies.herokuapp.com/graphql
- [✓] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
>![Successful Build](/assets/Success.png)
>![Successful Build Graph QL](/assets/Success1.png)
- [✓] Answer the **4** questions below.
- [✓] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Accessibility... Meaning that multiple people can use the container and if you are not at your local machine you can access the conatiner and work on your project away from your local machine.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> CircleCI runs and checks the program for any errors that would cause the system to fail entirely. It is basically a check to see if you coded correctly.
3. Why would you use a container technology over a virtual machine(VM)?
> First VM can be unstable and oyu would lose all of your work while a program like docker utilizes almost a cloud type arcitecture.
4. What are some alternatives to Docker for containerized deployments?
> Hyper-V and Windows COntainers, runC, and Podman are all alternatives. (Source: https://jfrog.com/knowledge-base/7-alternatives-to-docker-all-in-one-solutions-and-standalone-container-tools/)