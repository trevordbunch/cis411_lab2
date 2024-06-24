# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Garrett Nissley
**GitHub Handle:** ggn10
**Repository:** [ggn10/cis411  ](https://github.com/ggn10/cis411_lab3_uiux)   
**Collaborators:** None
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here:  
![http://cis411lab4-ggn10.herokuapp.com/graphql](https://cis411lab4-ggn10.herokuapp.com/)
![GraphQL](../assets/graphqlSS.PNG)
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
![Successful Build](../assets/ggn10ciSS.PNG)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Containerized versions of applications allow for great efficiency, fast delivery, and fast management.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> CircleCI allows us to continuously see how are app is being built and deployed. This will make troubleshooting and new commits easier.
3. Why would you use a container technology over a virtual machine(VM)?
> Container technology does not require a virtualized OS or a Hypervisor layer.
4. What are some alternatives to Docker for containerized deployments?
> Kubernetes.