# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2022  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Andrew Coldsmith  
**GitHub Handle:** [andrewcoldsmith](https://github.com/andrewcoldsmith)  
**Repository:** [Forked Repository](https://github.com/andrewcoldsmith/cis411_lab4_CD)  
**Collaborators:** [Grace Schlauder](https://github.com/grace-schl); [Michael Mourelatos](https://github.com/MichaelMourelatos)
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [ ] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> Example: ![Successful Build](../ex/trevordbunch_lab2_02.png)
- [ ] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it):  
> Example: [http://cis411lab2-trevordbunch.herokuapp.com/graphql](http://cis411lab2-trevordbunch.herokuapp.com/graphql)  
> ![Successful Test on Deployed URL](../ex/trevordbunch_lab2_01.png)
- [x] Answer the **4** questions below.
- [ ] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> The application may work on my computer, but that doesn't guarantee it will work on other computers. With containerization, everything the application is dependent on is kept in boxes that can be moved with the project to a new system.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> CircleCI runs tests on files when they are published and recognizes problems. This prevents developers from publishing broken code or incorrect files.
3. Why would you use a container technology over a virtual machine(VM)?
> Containers require far less storage than virtual machines. Also, they can easily be moved to any computer while VMs need to be set up on a system before the transferred application can be used.
4. What are some alternatives to Docker for containerized deployments?
> A few other popular containerizing software include AWS Fargate, Linux Containers (LXC), and Microsoft Azure.