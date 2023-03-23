# Lab Report: Continuous Deployment 
___
**Course:** CIS 411, Spring 2023  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Jonah Robinson  
**GitHub Handle:** [jrmakr2123](https://github.com/jrmakr2123)  
**Repository:** [Continuous Development](https://github.com/jrmakr2123/cis411_lab4_CD) 
<!-- **Collaborators:**  -->
___

# Required Content

- [x] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [x] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [x] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [x] Write the URL of your app hosted on Heroku or other Cloud Provider here:  [https://cis411lab4-jrmakr2123-u4el5.ondigitalocean.app/graphql](https://cis411lab4-jrmakr2123-u4el5.ondigitalocean.app/graphql)
- [x] Embed _using markdown_ a screenshot of your successful deployed application to Digital Ocean.  
> ![Successful Build](./../assets/digital%20ocean%20app.png)
- [x] Embed _using markdown_ a screenshot of your successful build and deployment to Digital Ocean of your project (with the circleci interface).  
> Example: ![Successful Build](./../assets/digital%20ocean%20circleci%20test.png)

<!-- You may want to consider adding this here professor -->

- [x] Copy your mutation from your graphql instance here: 
~~~
{
  "data": {
    "mutateAccount": {
      "id": "dd6073cc-2118-4927-8e34-9b369a8d781f",
      "name": "Jonah Robinson",
      "email": "jr1521@messiah.edu"
    }
  }
}
~~~
- [x] Answer the **4** questions below.
- [x] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?
> By having a containerized version of an application, the development team can run the same tests on the same containerized hardware. The application may be able to run with no errors on one computer, but on another it may not run. Containers make it possible for developers to have the same set of hardware to make changes. 
2. If we have the ability to publish directory to Digital Ocean, why involve a CI solution like CircleCI? What benefit does it provide?
> Where a continuous Integration program like CircleCI would help developers compile, test, and maintain usable code, Continuous Delivery would help developers deliver new codes and programs for more testing in more realistic situations. Were CI would be more focused on creating usable code, CD is more interested in delivering and monitoring that code for future fixes.  
3. Why would you use a container technology over a virtual machine(VM)?
> Container technology interfaces with the kernel thus not requiring an additional license to run. In virtual machine instances, licensing is required for each additional virtual machine. Another reason is that container technology does not require as much resources as virtualization. Containerization focusses on using what the computer is already giving in kernel manipulation thus allowing for a faster and lightweight running process. Virtualization focusses on partitioning a certain amount of computer resources. In doing so everything is recopied and ran through a compatibility layer. To get the performance of a container in a virtual machine the virtual machine would need more resources than the container would need in the first place. 
4. What are some alternatives to Docker for containerized deployments?
> Some alternatives to docker are . . .
> - Hyper-V Containers,
> - Containerd,
> - Kubernetes,
> - RunC,
> - Buildah,
> - and many more options for developers. 