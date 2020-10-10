# **Lab 1:** _Setting up **Node-RED** and **IBM Watson** on IBM Cloud_
You can install Node-RED locally on your own computer, on devices such as [Raspberry Pis](https://www.raspberrypi.org/) and [Arduinos](https://www.arduino.cc/), and in the cloud using services from IBM, Microsoft and Amazon. In this tutorial we will run Node-RED on the **IBM Cloud**. If you want to know more about setting up Node-RED in other environments, go [here](https://nodered.org/docs/getting-started/).

After we've installed Node-RED, we'll also use this lab to setup the **IBM Watson** AI services we're going to use in this tutorial.

## Part 1: Create Node-RED application
**(1)** Login to [IBM Cloud](https://cloud.ibm.com) and click on `Catalog` in the menu bar.

![](./images/ibmcloud-001.png)

**(2)** Search on 'node-red'.

![](./images/ibmcloud-002.png)

**(3)** Select `Node-RED App` from the drop down list.

![](./images/ibmcloud-003.png)

**(4)** When the 'Node-RED App' screen appears select the `Create` tab.

![](./images/ibmcloud-004.png)

**(5)** Select `London` in the `Region` field.

![](./images/ibmcloud-005.png)

**(6)** Wait for a short while until the application is ready to deploy.

![](./images/ibmcloud-006.png)

**(7)** Select the `Deploy your app` button when it is enabled.

![](./images/ibmcloud-007.png)

**(8)** Create a Cloud API Key by selecting `New` next to the highlighted field.

![](./images/ibmcloud-008.png)

**(9)** Create a new API key with full access by selecting `Ok`.

![](./images/ibmcloud-009.png)

**(10)** Select `Cloud Foundry` for the `Deployment target` then `Next`. Make sure `Region` is the same as the region selected in Step 5 (i.e. `London`).

![](./images/ibmcloud-010.png)

**(11)** In the `Configure the DevOps toolchain` screen make sure `Region` is the same as the region selected in Step 5 (i.e. `London`) then select `Create`. 

![](./images/ibmcloud-011.png)

**(12)** Wait for the `DevOps toolchain` to deploy, this can take several minutes so be patient!

![](./images/ibmcloud-012.png)

**(13)** Once the DevOps toolchain is deployed the status will change from `In progress` to `Success`. If this seems to be taking a while try refreshing the page. 

![](./images/ibmcloud-013.png)

**(14)** Select the `App URL` to launch Node-RED (again, refresh the page if this does not automatically appear). This will be something like https://node-red-effur-2020-09-09.mybluemix.net

![](./images/ibmcloud-014.png)

**(15)** The first time you log on to your new Node-RED application, you'll have to do small amount of configuration. On the first Welcome screen, hit `Next`.

![](./images/ibmcloud-015.png)

**(16)** On the next `Secure your Node-RED editor` screen, enter a `Username` and `Password` that you will use to login to your Node-RED application. You can use any name and password here, but please ensure you are careful typing in your password and that you remember it!

![](./images/ibmcloud-016.png)

**(17)** Answer `Next` to the next couple of questions and finally `Finish` and after a few seconds you'll be presented with the `Node-RED on IBM CLoud` screen. Click on `Go to your Node-RED editor`.

![](./images/ibmcloud-017.png)

**(18)** After a few moments, you'll see the Node-RED welcome screen. Login with the username and password you've just specified, and you'll be taken to your new Node-RED environment.

![](./images/ibmcloud-018.png)

**(19)** Congratulations! You can now start to build applications using Node-RED's visual editor. If at any time you want to find your Node-RED environment again (i.e. after logging out and back in. First go to the `Dashboard` view in IBM Cloud.

![](./images/ibmcloud-019.png)

**(20)** Click on your Node-RED application highlighted below.

![](./images/ibmcloud-020.png)

**(21)** Finally click on `Visit App URL` highlighted below.

![](./images/ibmcloud-021.png)

## Part 2: Create IBM Watson services
For the applications we are going to build in this tutorial, we need to access and use some of IBM Watson's AI services. Watson has a number of these services, but we are going to use just three of them here:

- Watson Natural Language Understanding
- Watson Visual Recognition
- Watson Language Translator

**(1)** We therefore need to provision an instance of each of these services for use by our apps. Within **IBM Cloud**, go back to the `Catalog`, select `AI` from the sidebar, and then `Natural Language Understanding`.

![](./images/09-nlu.png)

**(2)** On the next screen you can leave everything to the defaults, and hit `Create` to spin up your **Natural Language Understanding** (NLU) service.

_If you want to you can scroll down and change the `Service name` before you hit `Create`, but this isn't really necessary._

![](./images/10-nlu2.png)

**(3)** You'll now be taken to a `Getting Started` page for your NLU service. From here, click `Manage` on the sidebar and you'll see the services **security credentials**.

Each of the IBM Watson services you create has associated  **credentials** - this is a security measure to ensure that only you (or anybody you supply the credentials to) can use the service.

Click the `Copy to clipboard` icon to the right of the `API Key` field to copy the key, and then paste this in a document or note somewhere, then do the same with the `URL`. We'll need these later on when we're building our Node-RED apps.

![](./images/11-nlucreds.png)

**(4)** Now repeat this process to create both **Visual Recognition** and **Language Translator** services: select `Catalog`, then `AI` from the sidebar, click the respective service, then `Create` on the next screen.

Don't forget to save the security credentials for these two additional services too!

**OK that's setup done! Let's move onto creating our first Node-RED application. Click [here](../2-Hello-World) to go to Lab 2.**
