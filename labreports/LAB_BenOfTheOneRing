# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Ben Clarke 
**GitHub Handle:** BenOfTheOneRing  
**Repository:** [My Forked Repository](https://github.com/BenOfTheOneRing/cis411_lab4_CD.git)  
**Collaborators:** Mike Shoul, Grace Taylor via Pull request 
___

# Required Content

- [x] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
[Azure URL](https://labcd4app.azurewebsites.net/graphql)
- [x] Embed _using markdown_ a screenshot of your successful deployed application to Azure.  
![Successful Build](/1st_successful_build.png)
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Azure of your project (with the circleci interface).  
![Successful Deployment](/build_2.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?

> Because containerized applications contain all of their own data and app/file versions. This way if two devs have different versions of npm, git, or some other necessary file or service, those differences do not leak into errors with the app if the app is deployed to a different environment. 
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> It checks for errors and makes sure the app can actually run. This saves valuable time in troubleshooting, and also acts as a fail-safe in-case a dev accidentally sends a broken build to the deployed server. CircleCI would block that type of dangerous deployment. 
3. Why would you use a container technology over a virtual machine(VM)?
> Because a virtual machine, while it would stop your personal device from being harmed from errors, would still have environments that would most likely not match with every user's systems and environments. If an app fully contains its own dependencies then it does not matter what device it is used on. 
4. What are some alternatives to Docker for containerized deployments?
> Cloud Foundry, Containerd, CoreOS rkt, Kubernetes