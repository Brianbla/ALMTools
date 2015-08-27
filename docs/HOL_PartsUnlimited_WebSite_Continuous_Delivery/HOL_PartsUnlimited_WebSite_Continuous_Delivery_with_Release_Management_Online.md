HOL - Parts Unlimited WebSite Continuous Delivery with Visual Studio Online & Release Management Online
====================================================================================
In this lab we have an application called PartsUnlimited. We want to set up
Visual Studio Online to be able continuously deploy our built code to designated environments in our release pipeline. 
This means that whenever code is committed and pushed to the master branch, it will be built and that it will deploy correctly to the proper enviroment to get fast feedback. To do so, 
we are going to be using our Continuous Integration build (CI) that we built in a previous HOL and 
create a new Release Pipleine with Release Management Online using Visual Studio Online.

###Pre-requisites:###

-   An active Visual Studio Online account

-   An active Azure subscription

-   Project Admin rights to the Visual Studio Online account
 
### Tasks Overview: ###

**Set up your Visual Studio Online account:** This step helps you download the source code, and then push it to your own Visual Studio Online account.

**Create Continuous Delivery Pipeline:** In this step, you will create a release pipeline in Visual Studio Online that will be triggered every time a commit is pushed to your repository in Visual Studio Online. 

### Pre-Requisite: Connect to your Visual Studio Online account

We want to push the application code to your Visual Studio Online account in
order to use Build.

**1.** First, we need to open Team Explorer. Go to your **account home
page**:

	https://<account>.visualstudio.com

> **Talking Points:** If you need to learn how to setup a VSO account, click [https://www.visualstudio.com/en-us/get-started/setup/sign-up-for-visual-studio-online](https://www.visualstudio.com/en-us/get-started/setup/sign-up-for-visual-studio-online)

**2.** Connect to the VSO account project using Visual Studio.

![](<media/25.jpg>)
