# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Noah Calisti  
**GitHub Handle:** [noahcal11](https://github.com/noahcal11)  
**Repository:** [My Repository](https://github.com/noahcal11/cis411_lab4_CD)  
**Collaborators:** 
___

# Required Content

- [X] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [X] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [X] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [ ] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
> Example: [http://cis411lab2-trevordbunch.herokuapp.com/graphql](http://cis411lab2-trevordbunch.herokuapp.com/graphql)
- [ ] Embed _using markdown_ a screenshot of your successful deployed application to Heroku.  
> Example: ![Successful Build](../ex/trevordbunch_lab2_01.png)
- [ ] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> Example: ![Successful Build](../ex/trevordbunch_lab2_02.png)
- [ ] Answer the **4** questions below.
- [ ] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Containers package an application and all of its dependencies into one portable unit. If I test locally, my application may work on my machine but cause errors on someone else's. By running in a container, the entire team can develop in the same reliable environment.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> CI solutions allow for automation and feedback. Automating the building, testing, and deployment processes allows developers to focus elsewhere rather than configuring deployment settings. CI tools also provide much faster feedback on when code changes cause issues so developers can fix issues sooner. These allow for greater scalability as applications grow in complexity and size.
3. Why would you use a container technology over a virtual machine(VM)?
> Containers are much more efficent than VMs. They use the native OS instead of a separate one, meaning they require much less resources. They can run on any machine that supports the container runtime. It is both more cost and time efficent to use containers over VMs.
4. What are some alternatives to Docker for containerized deployments?
> Alternatives to Docker include Podman, CRI-O (for Kubernetes), LXC/LXD (for Linux), rkt, and OpenVZ