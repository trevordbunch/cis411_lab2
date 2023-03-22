# Lab Report: UX/UI
___
**Course:** CIS 411, Spring 2023  
**Instructor(s):** [Trevor Bunch](https://github.com/trevordbunch)  
**Name:** Grace Taylor  
**GitHub Handle:** gracet712  
**Repository:** https://github.com/gracet712/cis411_lab4_CD  
**Collaborators:**  N/A
___

# Required Content

- [X] Generate a markdown file in the labreports directory named LAB_[GITHUB HANDLE].md. Write your lab report there.
- [X] Create the directory ```./circleci``` and the file ```.circleci/config.yml``` in your project and push that change to your GitHub repository.
- [X] Create the file ```Dockerfile``` in the root of your project and include the contents of the file as described in the instructions. Push that change to your GitHub repository.
- [X] Write the URL of your app hosted on Heroku or other Cloud Provider here:  
[https://lab04app.azurewebsites.net/graphql](https://lab04app.azurewebsites.net/graphql)
- [X] Embed _using markdown_ a screenshot of your successful deployed application to Azure.  
![Successful Build - Azure](/assets/successful_deploy_azure.png)
- [X] Embed _using markdown_ a screenshot of your successful build and deployment to Azure of your project (with the circleci interface).  
![Successful Build - CircleCI](/assets/successful_circleci_azure_deploy.png)

![Successful Build - Azure](/assets/azure_build_success.png)

![Working App](/assets/final_working_app.png)
- [X] Answer the **4** questions below.
- [X] Submit a Pull Request to cis411_lab4_CD and provide the URL of that Pull Request in Canvas as your URL submission.

## Questions
1. Why would a containerized version of an application be beneficial if you can run the application locally already?

> There are at least two potential ways to answer this question - first, a cloud version of an application is superior to a local version because it is always available regardless of whether your local system is turned on, and does not require you to acquire a public IP address yourself (the cloud provider does this) for others to access it. It is also backed up, and cloud service providers offer some level of security/additional services to support your application. It is also possible to scale up and down quickly to support changing needs.

> Second, a containerized version is beneficial because it takes up fewer resources for a single application than a full VM. A business might run many containers within a single VM, allowing them to isolate specific applications for security purposes without needing to waste resources replicating the entire OS for every container.

> IBM explains the benefits of hosting applications in the cloud here: https://www.ibm.com/topics/cloud-computing-benefits

2. If we have the ability to publish directory to Azure, why involve a CI solution like CircleCI? What benefit does it provide?

> CircleCI automatically runs tests on the application before it is deployed to Azure. If the tests don't pass, then the changes are not published to Azure. This prevents many bugs and errors from being published and potentially causing problems to users. This is the point behind CI/CD.

> CircleCI explains much of this here: https://circleci.com/continuous-integration/

3. Why would you use a container technology over a virtual machine(VM)?

> As explained in question 1, container technology solves a conflict between security and efficient use of resources. If using VMs, a company faces the choice between putting multiple applications on a single VM - thereby making it likely that all of those applications will be compromised if a single one is compromised - or conforming to good cybersecurity practices and putting each application on a separate VM. However, if the company does this, they will be wasting resources by replicating the OS on every VM. Containers isolate applications, but are more lightweight than VMs, solving both problems.

> According to IBM, some additional benefits to containers include:
- Portability
- Agility
- Speed
- Fault Isolation
- Efficiency
- Ease of Management

> This information can be found here: https://www.ibm.com/topics/containerization

4. What are some alternatives to Docker for containerized deployments?
> According to IBM, some alternatives include:
- containerd
- CoreOS rkt
- Mesos Containerizer
- LXC Linux Containers
- OpenVZ
- crio-d

> This information can be found here: https://www.ibm.com/topics/containerization

## Extra Credit - Azure Instructions

Note - Azure for Students does not require a credit card

### In Step 0: for set-up

1. Sign up for an Azure Students account: https://azure.microsoft.com/en-us/free/students/

2. Download and install the Azure CLI: https://learn.microsoft.com/en-us/cli/azure/install-azure-cli


### In Step 4 - Set up an Azure application

1. Go to your Azure Home page - click "Home" in the upper left corner of the default welcome page - and Click "Create a resource."

2. Select "Containers" on the left menu, and then "Container Registry."

3. Fill out the registry creation information. You will probably need to create a new resource group - I called mine "Labs-Group." Pick a registry name. For instance, mine is "cislabsregistry." Other settings can be left at default.

4. Click "Review + Create" and then "Create."

5. Go to the root of your project directory. Run:

```az acr build --registry <container_registry_name> --image <name_of_image> .```

Note the dot at the end. Use your registry name and any name you choose for the image (I chose lab4). This command may take a minute or two.

6. You may be prompted to login by running az login. This will open a browser window where you log in with your student account. You can then close the window and return to the command line, where you will be logged in. Re-run the command in step 5.

7. To view the image you created, go to your Azure resources page in the portal. Click your registry, then click "Repositories" from the "Services" section on the left.

8. To deploy the application, you need to enable Docker access in Azure Container Registry. This step allows the Azure App service to access the containers stored in the registry. From your Resources page, click the registry to open its overview page (you should already be here). From the Settings section (on left) click Access keys.

9. Enable "Admin User." A username and some passwords will be displayed.

10. Click "Home," then "Create a resource." Select "Web app."

11. Fill out the web app information. Same resource group as before. Choose a name for your app (I chose lab04app). For Publish, choose "Docker Container." For OS, choose Linux. The default pricing plan will be Basic B1 - about 12.41/month. You should have $100 free credits with your student account, so leaving this option should be fine. I chose to try to the free pricing plan anyway with 60 min CPU time per day, and this also worked fine.

12. Click "Next: Docker."

13. Docker page:
- Single Container option
- Image Source: Azure Container Registry
- Enter your registry name in the Registry field
- Enter your image in the image field
- For Tag, select "latest"
- Leave Startup Command empty - this is done in Dockerfile.

14. Click Review + create, then Create.

15. Visit http://[YOUR_WEB_APP_NAME].azurewebsites.net/graphql. You may need to wait for a while before this loads.



### In Step 5 - Integrate with CircleCI

1. Go to your Azure Resources page and click your web app name to open the Overview page. From the side menu, pick Deployment Center. Scroll down to Continuous Deployment and select On. Then click Save. With continuous deployment selected, the web app will trigger a new deployment of the Node.js application each time the Docker image is rebuilt on Azure Container Registry.

2. On GitHub, create a new branch called "deploy."

3. From your CircleCI project, click Project Settings, (top right of the page) then SSH Keys (on the side menu).

4. In the User Key section, click Authorize with GitHub. Authenticate with GitHub to finish this process.

5. Go back to the SSH Keys section, and click Add User Key. Save the generated key in a safe location for the next step.

6. From the side menu on the Project Settings, click Environment Variables. Add these environment variables:
- GITHUB_EMAIL: email connected to your GitHub account
- GITHUB_USERNAME: your GitHub username
- GITHUB_FINGERPRINT: the key you just saved

7. Next, we will generate a GitHub personal access token. Go to GitHub, then choose Settings > Developer Settings (at the bottom of the menu on the left). Select "Personal access tokens." (classic, not Beta) Click "Generate a personal access token."

8. Enter a description, grant all permissions except delete_repo, and Click "Generate token." I left the expiration at 30 days as that should be plenty of time for this lab. Copy and/or save the token; it will not be displayed again after you leave the page.

9. Next, go to the root of your project (in the command line) and run the following command:

```az acr task create --registry <container_registry_name> --name buildnodeapp --image mynodeimage --context <your_github_repo>#deploy --file Dockerfile --git-access-token <access_token>```

Replace the registry name with your registry name, name the task whatever you like, replace the image name with your image name, the GitHub repo with the URL to the root of your repo on GitHub, and add your access token at the end. This command creates a task in Azure to monitor the deploy branch for updates and rebuild the image every time updates are pushed. We will later make a script to push updates from the purelab branch to the deploy branch when they pass CircleCI validation.

10. To view the newly created task, go to the overview page on Azure for your registry and click Tasks in the Services section on the left-hand menu. The task should then be displayed on the right with the name you gave it.

11. Run the following at the root of your project directory:

```npm install gh-pages --save-dev```

And add the following in the package.json file:

```
"scripts" : {  
  ...   
  "deploy" : "npx gh-pages -b deploy --message '[skip ci] Updates' -d ./"   
}
```

You will add the "deploy..." line in the scripts section that already exists.

This provides setup for any changes pushed to purelab to be sent first to CircleCI, and then only pushed to the deploy branch and built on Azure if they pass those tests.

12. Next, add the following to your config.yml file:
```
deploy:
    working_directory: ~/repo
    docker:
      - image: circleci/node:11
    steps:
      - checkout
      - run:
          name: Configure Github credentials
          command: |
            git config user.email $GITHUB_EMAIL
            git config user.name $GITHUB_USERNAME
      - add_ssh_keys:
          fingerprints:
            - $GITHUB_FINGERPRINT
      - run:
          name: Deploy to Azure Web App Using Azure Container Registry Task
          command: npm run deploy

workflows:
  version: 2
  build:
    jobs:
      - build
      - deploy:
          requires:
            - build # only deploy once build job has completed
          filters:
            branches:
              only: purelab # only deploy on the main branch
```

Note that "deploy" is a second job and should be in line with "build" (already in file). "workflows" should be aligned to the far left.

12. Save, commit, and push changes. You should see the tests complete successfully on CircleCI (for purelab branch). In Azure, if you go into your registry and select Services > Tasks from the left, then switch to the Runs tab, you should see the image be successfully rebuilt there.

13. Now, every time you commit to the purelab branch, it will be pushed to CircleCI, tested, then automatically pushed to the deploy branch, which Azure will automatically detect and then rebuild the image. Note that the .circleci directory will not show up in the deploy branch, which may cause an error on CircleCI - but the purelab branch has already been tested and the web app runs fine on Azure.

Instructions are a modified version of this tutorial:
https://circleci.com/blog/deploying-container-based-node-apps-to-azure/