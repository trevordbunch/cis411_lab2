# Lab Report: Container
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Annika Kowalski  
**GitHub Handle:** AnnikaKowalski   
**Repository:** https://github.com/AnnikaKowalski/cis411_lab4_CD    
**Collaborators:** 
___

# Required Content

- [ ] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [ ] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [ ] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [ ] Write the URL of your running Heroku app here:  
> Example: [http://cis411lab2-trevordbunch.herokuapp.com/graphql](http://cis411lab2-trevordbunch.herokuapp.com/graphql)
- [ ] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> Example: ![GraphiQL_SC](/assets/GraphiQL_SC.png)
    
- [ ] Answer the **4** questions below.
- [ ] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
    - A container allows members working on the project to run the application without needing to install/download any other software or programs. The container also contains all of the programs/dependencies needed for the program to run. 
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
    - CircleCI is the middle man for the project. It tests and deploys the program to ensure that it is working properly. It also allows multiple ensures to push their code before it goes live on Heroku. 
3. Why would you use a container technology over a virtual machine(VM)?
    - Containers are used more often than virtual machines because containers take up less space than the virtual machines do. Virtual machines are often times more dependant and typically also take longer to set up than container do. 
4. What are some alternatives to Docker for containerized deployments?
    - Some alternatives to Docker are LXD, rkt and Mesos. 