# Lab Report: UX/UI

___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Micah Johnson  
**GitHub Handle:** mcjo163  
**Repository:** [mcjo163/cis411_lab4_cd](https://github.com/mcjo163/cis411_lab4_cd)  
**Collaborators:** Annika Kowalski
___

## Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here:  

> Example: [http://cis411lab4-mcjo163.herokuapp.com/graphql](http://cis411lab4-mcjo163.herokuapp.com/graphql)

- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.

> Example: ![Successful Build](/assets/success.png)

- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions

1. Why would a containerized version of an application be beneficial if you can run the application locally already?
    > Using a containerized environment increases consistency and flexibility. Different people's local setups may differ, and so having an identically configured container environment will ensure that everyone sees the same thing on their end as well. Also, these consistent environments lend themselves very nicely to automation.

2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
    > Publishing directly to Heroku would skip over the CI part of CI/CD. The integration and build processes are important as well and that is the first thing we are using CircleCI for, so we should not skip over it.

3. Why would you use a container technology over a virtual machine(VM)?
    > Containers are much lighter and do not require nearly as much overhead as VMs do. Using VMs would be overkill and wasteful, when container technology is an option.

4. What are some alternatives to Docker for containerized deployments?
    > According to StackShare, some popular alternatives include LCX, rkt, Kubernetes, Cloud Foundry, Vagrant, Red Hat OpenShift, VirtualBox, and containerd.
