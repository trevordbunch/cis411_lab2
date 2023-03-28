# Lab Report: CD
___
**Course:** CIS 411, Spring 2023  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Jonathan Gaston 
**GitHub Handle:** JG1579  
**Repository:** https://github.com/JG1579/cis411_lab4_CD?organization=JG1579&organization=JG1579
**Collaborators:** 
___

# Required Content

- [ /] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [/ ] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [/ ] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [/ ] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
>  [http://seahorse-app-6jogq.ondigital.app/graphql](https://seahorse-app-6jogq.ondigitalocean.app/graphql?query=mutation%20%7B%0A%20%20mutateAccount(input%3A%20%7B%0A%20%20%20%20email%3A%20"JG1579"%0A%20%20%20%20name%3A%20"Jonathan%20Gaston"%0A%20%20%20%20mutation%3A%20"add"%0A%20%20%7D)%20%7B%0A%20%20%20%20id%0A%20%20%20%20name%0A%20%20%20%20email%0A%20%20%7D%0A%7D%0A)
- [ /] Embed _using markdown_ a screenshot of your successful deployed application to Heroku.  
>  ![Successful Build](/assets/digital%20ocean%20verify.jpg)
- [/ ] Embed _using markdown_ a screenshot of your successful build and deployment to Digital Ocean of your project (with the circleci interface).  
> ![image](/assets/verify%20graphql.jpg)

- [ ] Answer the **4** questions below.
- [ ] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> Containers are more lightweight then V.m's and therefore are faster to start up. This means you can test and adjust apps quickly.
>Containers keep dependencies and config's and so they give a more consistent experience throughout development.
>They make it easier to use microservice architecture.
>They are easy to deploy on various platforms
2. If we have the ability to publish directory to Digital Ocean, why involve a CI solution like CircleCI? What benefit does it provide?
> CircleCI tests the code before deployment preventing you from sending broken code out.
> Allows you to test multiple programs at the same time. This saves time foe developers as they can know what works and what needs to be fixed.
>Allows for multiple extensions giving developers a wider array of tools.
>Lets you customize the workflow giving developers a greater amount of control for testing.
3. Why would you use a container technology over a virtual machine(VM)?
> They are faster to load up as they only deploy the app and not the entire OS 
>They are more efficient, as stated above the resources are focused on the app only and not the entire OS.
>They are easier to deploy on the cloud.
4. What are some alternatives to Docker for containerized deployments?
> Containerd: open source daemon that works as a interface for the container process. Works with Linux and Windows and is known for easy to mange container lifecycle
>Cloud Factory: Open source and industry level cloud app platform. Can use multiple different programming languages and uses your computers infrastructure to deploy apps.
>Hyper-V Containers:They are not open sources although they are compatible with open source solutions. They provide a good degree of isolationism and portability.