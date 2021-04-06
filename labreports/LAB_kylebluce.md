# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Kyle Luce  
**GitHub Handle:** https://github.com/kylebluce  
**Repository:** https://github.com/kylebluce/cis411_lab4_CD  
**Collaborators:** @scribhneoir
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here: http://cis411lab4-kylebluce.herokuapp.com/graphql
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
![Successful Build](/assets/HerokuGraphql.PNG)
![CircleCI Success](/assets/CircleCI1.PNG)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?

A containerized version of an application would allow for collabortation to run more smoothly. More people could have access to work on the application at the same time rather than the application just working on one machine.

2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?

CI solutions like CircleCI have the ability to detect errors in published code and allow for quick changes of that code. CircleCI also allows for more feedback from users by seeing which updates customers liked and which updates caused customers to stop using the application.

3. Why would you use a container technology over a virtual machine(VM)?

Container technology is more cost effective since most container technologies are Open Source. They also tend to be more scalable because of their quick boot speeds and low downtime. Lastly, they have more security built into the containers whereas you would have to put more resources into protecting a virtual machine.

4. What are some alternatives to Docker for containerized deployments?

The one I heard of the most while looking at different websites for this lab was Kubernetes, and I found another one called rkt. According to Microsoft, "Kubernetes is meant to run across a cluster while Docker runs on a single node." Rkt, also called CoreOS Rkt, tends to be more secure than docker, and it is probably docker's biggest competition.
