# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Joe Vera  
**GitHub Handle:** JoeV22 
**Repository:** [My Forked Repository](https://github.com/JoeV22/cis411_lab4_CD)  
**Collaborators:** @RomanSearle @trevorbunch
___

# Required Content

- [Yes] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [Yes] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [Yes] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [Yes] My URL for running Heroku app here:  
> My URL: [https://cis411lab4-joev22lab4.herokuapp.com/graphql](https://cis411lab4-joev22lab4.herokuapp.com/graphql)
- [Yes] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> Example: ![Successful Build](../assets/herokuworks.png)
> Example 2: ![Successful Build - look at top one](../assets/builddeployworkflow.png)
- [Yes] Answer the **4** questions below.
- [Yes] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Sometime's it's important to be able to deploy it inside a container in order to run specific tests on it.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Most of our build configurations are within the yml file. So if you need to edit it to do variations it's much more preferable to do it from a CI solution. One of the things that makes it stand out is it's speed, this helps us run complex pipelines faster than heroku.
3. Why would you use a container technology over a virtual machine(VM)?
> Containters are much faster and agile than virtual machine proving to handle complex tasks with ease, outpacing virtual machines.
4. What are some alternatives to Docker for containerized deployments?
>  Windows container, linuxV server and LXD are all viable containerized deployment alternatives to docker.