HOL - Parts Unlimited WebSite Continuous Delivery with Visual Studio Online & Release Management Online
====================================================================================
In this lab we have an application called PartsUnlimited. We want to set up
Visual Studio Online to be able continuously deploy our built code to designated environments in our release pipeline. 
This means that whenever code is committed and pushed to the master branch, it will be built and that it will deploy correctly to the proper enviroment to get fast feedback. To do so, 
we are going to be using our Continuous Integration build (CI) that we built in a previous HOL and 
create a new Release Pipleine using Release Management Online using Visual Studio Online.

###Pre-requisites:###

-   An active Visual Studio Online account

-   An active Azure subscription

-   Project Admin rights to the Visual Studio Online account
