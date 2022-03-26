# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Abigail Garrido  
**GitHub Handle:** ag1454  
**Repository:** https://github.com/ag1454/cis411_lab4_CD  
**Collaborators:** none
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> ![Successful Build](/assets/herokusuccess.png)
- [x] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it): http://cis411lab4-ag1454.herokuapp.com/graphql
> ![Graphql](/assets/herokugraphql.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> If this is an application that only you are working on, running it locally is fine and dandy. For applications being worked on by a team of people, a containerized version of it is better because then it is more accessible; everyone in the team, including you, would be able to access it without needing the local machine.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Involving something like CircleCI allows for an error-check before publishing directly to Heroku.
3. Why would you use a container technology over a virtual machine(VM)?
> If using a virtual machine, an entire virtual machine would be needed for each app, and that can be too many "parasites" for the computer to sustain.
4. What are some alternatives to Docker for containerized deployments?
> Some alternatives are Podman, OpenVZ, and VirtualBox (source: https://rigorousthemes.com/blog/best-docker-alternatives/).
