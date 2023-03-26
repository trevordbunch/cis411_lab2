# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Mitch DiFante
**GitHub Handle:** @mitchdifante
**Repository:** https://github.com/mitchdifante/cis411_lab4_CD.git 
**Collaborators:** 
___

# Required Content

- [x] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.

- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.

- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
  
- [x] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
> Example: [http://cis411lab2-trevordbunch.herokuapp.com/graphql](http://cis411lab2-trevordbunch.herokuapp.com/graphql)

> (http://mitchdifante.herokuapp.com/graphql)

- [ ] Embed _using markdown_ a screenshot of your successful deployed application to Heroku.  

> Example: ![Successful Build](../ex/trevordbunch_lab2_01.png)

> ![Successful Build] (mutation {
>   mutateAccount(input: {
>   email: "md1430@messiah.edu"
>   name: "MITCH DIFANTE" 
>   mutation: "add"}) { 
>   id "b91950bd-5a99-4c58-8382-e48c67890756"
>   name "MITCH DIFANTE"
>   email "md1430@messiah.edu }}) 

> (My GraphiQL was not working throughout this, my npm items would constantly show up as errors. For time constraints I unfortunately could not get it squared away on my laptop.)

- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface). 

> Example: ![Successful Build](../ex/trevordbunch_lab2_02.png)

> ![Successful Build] (CircleCIScreenshot.png) (I was having several permission issues throughout this section and it would not take my file originally so it keeps failing).

- [x] Answer the **4** questions below.
  
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?


> Respond here... A containerized version of an application would be beneficial because it allows developers to write applications once and run them everywhere. Additionally, containers allow for the isolation of each app so there are no unanticipated interactions between different items which can ruin a test. Finally, containerized versions of applications can be much more consistent across different platforms.

2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?


> Respond here... The benefit that CircleCI provided instead of just publishing directory to something like Heroku is to provide a simple continuous delivery workflow for your organization.

3. Why would you use a container technology over a virtual machine(VM)?


> Respond here... We would use container technology over a virtual machine because containers require less to run than virtual machines. Additionally, container technology makes sense for a user planning to run multiple processes simultaneously compared to a virtual machine. Another reason to why we would prefer to use container technology rather than a virtual machine is containers do not need a Guest OS for every instence. Containers instead leverage the features and resources of the host OS. Overall, there are several factors that are much more appealing to us with container technology rather than virtual machines.

4. What are some alternatives to Docker for containerized deployments?


> Respond here... Some alternatives to Docker for containerized deployments are ones such as Cloud Foundry, Containerd, and LXC Linux Containers. Cloud Foundry is a pen-source, industry-standard cloud application that supports most programming languages and developer frameworks. Cloud Foundry can run apps on an IaaS Azure, AWS, GCP, OpenStack, or vSphere. Containerd is a open-source daemon. It works as an interface between your container engine and container runtimes. It is only supported by Linux and Windows, but makes it easy to manage container lifecycles. Finally, LXC Linux Containers is an open-source set of low-level container management resources designed to offer isolated application environments that function like virtual machines, but without the requirements needed to run their own kernel. The difference between this and Docker is that LXC Linux Containers allows a user to run more than one process in a single LXC container. LXC Linux Containers is ideal for traditional application design.