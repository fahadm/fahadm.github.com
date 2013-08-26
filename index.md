---
layout: page
title: Deploying your Application on AppHarbor!
tagline: Using git
---

## Deploying Your .net Application to Appharbor using git

I have noticed that many people new to git seem to have problems uploading their application to Appharbor.
For this tutorial i am going to use Github .

1. First of All make an account on Github https://github.com/ or Bitbucket https://bitbucket.org/
1a. If you are using Github request for private repositories using https://github.com/edu (you would get the private repositories instantly if you use university email)
2. Go to github.com and click New repository.
3. Enter the repository name , the description and click the private radio button, after all this click create the repository
4. Install git using http://windows.github.com/
5. Create a new directory with the name of your repository.
6. Open your project in Visual studio, under the build tool-bar click publish , enter the location of the directory which you had set the in previous step,
7. Open GitShell change the directory to directory created above.
8. Write the following commands:


> git config --global user.name ="username"

> git config --global user.email ="email"

> git init

> git add .

> git commit -m "First Commit"

> git remote add origin https://github.com/username/repositoryname.git

// For example this would be for me https://github.com/fahadm/fastshop.git

> git push -u origin master



When you would push it should ask for a password. enter your github password.
Now your Repository is ready. 

9. Create an account on https://appharbor.com.
10.After logging in to appharbor enter the name of your application then click create new.
11. Click settings on the left menu.

12. Click Disable Precompilation.

13.Click Configure GitHub to deploy to AppHarbor.

14. Select the repository you want to deploy from the drop down menu

15. In a few seconds your website will be deployed, you can access it using the name.apphb.com where name is the name which you used in step 10.


if you are using bitbucket just create a private repository in bitbucket and then in step 8 use the link provided by bit bucket 
$ git remote add origin https://username@bitbucket.org/username/repository.git 
Similarly in step 13 click configure using bitbucket
All the other steps are same

Screenshots to follow (Provided i get the time)
Happy Coding :).. 
Siging off
