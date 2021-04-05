# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2021  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Roman Searle <br>
**GitHub Handle:** RomanSearle <br>
**Repository:** [[https://github.com/RomanSearle/cis411_lab4_CD]](https://github.com/RomanSearle/cis411_lab4_CD) <br>
**Collaborators:** @el1303 and @JoeV22 
The Whole Lab
___

# Required Content

- [x] Generate a markdown file in the labreports directoy named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your running Heroku app here: https://cis411lab4-romansearle.herokuapp.com/graphql  
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Heroku of your project.  
> ![Successful Build](/assets/herokuProof.PNG)
> ![Successful BuildCircleCI](/assets/DeployProof.PNG)
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that ull Request in Canvas as your URL submission.


## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> A containerized version of an application would be beneficial over a locally running application because you can run tests in a container. 
2. If we have the ability to publish a directory to Heroku, why involve a CI solution like CircleCI? What benefit does it provide?
> Our build configurations are in the yml file. This allows us to do variations of builds on different branches. CircleCI is very fast. 
3. Why would you use a container technology over a virtual machine(VM)?
> Containers are faster, able to be changed quickly, and are more portable than VMs. 
4. What are some alternatives to Docker for containerized deployments?
> Kubernetes, Container Linux, and Apache Mesos are alternatives to Docker.

Refernces:
* https://blog.netapp.com/blogs/containers-vs-vms/

* https://cloudblogs.microsoft.com/opensource/2018/04/23/5-reasons-you-should-be-doing-container-native-development/

* https://www.toptal.com/kubernetes/what-is-kubernetes