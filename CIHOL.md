HOL - Parts Unlimited WebSite Continuous Integration with Visual Studio Online Build
====================================================================================
In this lab we have an application called PartsUnlimited. We want to set up
Visual Studio Online to be able continuously integrate code into the master
branch of code. This means that whenever code is committed and pushed to the
master branch, we want to ensure that it integrates into our code correctly to
get fast feedback. To do so, we are going to be setting up a Continuous Integration build (CI) that
will allow us to compile and run unit tests on our code every time a commit is
pushed to Visual Studio Online.

###Pre-requisites:###

-   An active Visual Studio Online account

-   An active Azure subscription

-   Project Admin rights to the Visual Studio Online account

### Tasks Overview: ###

**Set up your Visual Studio Online account:** This step helps you download the source code, and then push it to your own Visual Studio Online account.

**Add PartsUnlimited source to the Main Repo:** In this step, you will create a new Windows machine, install all the dependencies required to be a build machine, and then configure a build agent on it.

**Create Continuous Integration Build:** In this step, you will create a build definition in Visual Studio Online that will be triggered every time a commit is pushed to your repository in Visual Studio Online. 

### Pre-Requisite: Set up your Visual Studio Online account

We want to push the application code to your Visual Studio Online account in
order to use Build.

**1.** First, we need to open Team Explorer. Go to your **account home
page**:

	https://<account>.visualstudio.com

> **Talking Points:** If you need to learn how to setup a VSO account, click 

**2.** Connect to the VSO account project

### 1: Using own VSO to host Parts Unlimited Project

**1.** Navigate to [https://github.com/Microsoft/PartsUnlimited/tree/aspnet45](https://github.com/Microsoft/PartsUnlimited/tree/aspnet45) and download the sample as a zip

> **Talking Points:** For this lab is vitally IMPORTANT THAT YOU GET THE 4.5 BRANCH! If you want to use this locally you can https://github.com/Microsoft/PartsUnlimited/tree/aspnet45 and download the sample as a zip

**2.** Create folder to `C:/Source/HOL` and save the download to this folder.

**3.** Unzip the PartsUnlimited project, when unzipping be sure and “Unblock” the content or the deployment scripts won’t run

![](<media/21.jpg>)

**4.** Clone the repo of your team project to the location (`C:/Source/HOL`) where you extracted the sample

**5.**


### 2. Create Continuous Integration Build

A continuous integration build will give us the ability check whether the code
we checked in can compile and will successfully pass any automated tests that we
have created against it.

**1.** Go to your **account’s homepage**: https://<account\>.visualstudio.com

**2.** Click **Browse** and then select your team project and click
**Navigate**.

![](<media/22.jpg>)

**3.** Once on the project’s home page, click on the **Build** hub at the top of
the page.

![](<media/23.jpg>)

**4.** Click the **green “plus” sign**, select **Visual Studio Build**, and then click **OK**.

![](<media/24.jpg>)

> **Talking Points:** As you can see, you can now do Xamarin Android/IOS and Builds as well as Xcode builds.

**5.** Click on the **Repository** tab, and choose the git repository that
PartsUnlimited source is in.

**6.** We are going to use the **HOL** branch on the Repository tab

> **Talking Points:** We have multiple repos and branches, so we need to select the correct Repo and Branch before we can select which Solution to build.

**7.** Click on the **Build** tab, and click the ellipsis in the Build Solution pane.
