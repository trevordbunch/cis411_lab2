# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Rachel Beattie
**GitHub Handle:** [Your GitHub Handle](https://github.com/R-B1509/cis411_lab4_CD)  
**Repository:** [Your Forked Repository](https://github.com/R-B1509/cis411_lab4_CD)
**Collaborators:** 
___

# Required Content

- [x] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [ ] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
> Example:  ![URL](http://cis411lab4r09.azurewebsites.net/graphq)
- [ ] Embed _using markdown_ a screenshot of your successful deployed application to Azure.  
> Example: ![Azure](/cis411_lab4_CD/assets/cislab411azMu.png)
- [ ] Embed _using markdown_ a screenshot of your successful build and deployment to Azure of your project (with the circleci interface).  
> Example: ![CircleCI](/cis411_lab4_CD/assets/cislab411ccDeployment.png)
- [ ] Answer the **4** questions below.
- [ ] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> In case the local version freaks out or is going to crash, that way you can contain the damage.
2. If we have the ability to publish directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> It tests the publication before deployment, to see if there may be issues.
3. Why would you use a container technology over a virtual machine(VM)?
> It's faster than VM. VM involves swapping RAM from the Harddrive in a separate OS/Drive, which is slower in process but tricks the computer into believing there is more memory than physical. Container allows for the memory used in the Harddrive without needing to swap from another "virtual" drive that still relies on it. It also won't take up so much RAM because it's using another OS.
4. What are some alternatives to Docker for containerized deployments?
> LXC, Hyper-V, Windows Containers are a few examples.