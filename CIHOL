HOL - Parts Unlimited WebSite Continuous Integration with Visual Studio Online Build
====================================================================================
In this lab we have an application called PartsUnlimited. We want to set up
Visual Studio Online to be able continuously integrate code into the master
branch of code. This means that whenever code is committed and pushed to the
master branch, we want to ensure that it integrates into our code correctly to
get fast feedback. To do so, we are going to be setting up a build agent that
will allow us to compile and run unit tests on our code every time a commit is
pushed to Visual Studio Online.

###Pre-requisites:###

-   An active Visual Studio Online account

-   An active Azure subscription

-   Project Admin rights to the Visual Studio Online account

### Tasks Overview: ###

**Set up your Visual Studio Online account:** This step helps you download the source code, and then push it to your own Visual Studio Online account.

**Set up Windows virtual machine in Azure as the Build Agent:** In this step, you will create a new Windows machine, install all the dependencies required to be a build machine, and then configure a build agent on it.

**Create Continuous Integration Build:** In this step, you will create a build definition in Visual Studio Online that will be triggered every time a commit is pushed to your repository in Visual Studio Online. 

### Pre-Requisite: Set up your Visual Studio Online account

We want to push the application code to your Visual Studio Online account in
order to use Build.

**1.** First, we need to enable secondary credentials. Go to your **account home
page**:

	https://<account>.visualstudio.com
