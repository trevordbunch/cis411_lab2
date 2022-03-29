# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Thomas McVey  
**GitHub Handle:** ThomasMcVey  
**Repository:** https://github.com/ThomasMcVey/cis411_lab4_CD.git
**Collaborators:** 
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project (with the circleci interface).  
> Example: ![Successful Build](/assets/CIBuild.png)
> Had an issue with expected version being 11.X.
- [x] Write the URL of your running Heroku app here (and leave the deployment up so that I can test it):  
> Example: [http://cis411lab4-thomasmcvey.herokuapp.com/graphql](http://cis411lab4-thomasmcvey.herokuapp.com/graphql)
> ![Successful Test on Deployed URL](/assets/GraphMut.png)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> I would say because it helps standardize the environment, so to speak. Variation and uncertainty makes it hard to test code, so to have a way to know how the program reacts in a specific setting is easier to work with.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> It thoroughly goes through the tests made for it and thus may hit upon an error otherwise undetectable to our fallible, human senses.
3. Why would you use a container technology over a virtual machine(VM)?
> They virtualize only the most important bits and thus cut down on memory / resource costs.
4. What are some alternatives to Docker for containerized deployments?
> Podman, OpenVZ, and VirtualBox