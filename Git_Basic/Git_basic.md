**What is Git and GitHub?**

GIT stands for Global Information Tracker. GIT is basically version control system. For example if I create any file and then I changed or overwrite anything then the 1 st file will be my version one and then new will be version 2. This is done by GIT

There are two types of version control system. DVCS and CVCS these are two types. DVCS is distributed version control system and CVCS is centralised version control system. Example of CVCS is SVN and DVCS is GIT. 

You store your stuff in Repository. You can store any file. Repository is folder. Every repository of GIT is version controled. 

**If Repo is situated in your Computer then it is Local Repository**.

**If Repo is situated on different server  then it is Remote Repository.**

There are three stages is VCS.

1. FileSystem

2. Staging

3. VCS

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/482069e1-832c-4547-a360-07e057c687ad)

So when user created any file if he want initialise in local repo then use below command.

**Note: Neveruse git inside home directory. Create new directory and do init in that directory.**

**#git init**

When user want to add this file in staging area them use

**#git add**

When user want to send to the VCS them use.

**#git commit**

If user want file back from staging area to it local then use

**#git rm or uncheck**


Steps to install GIT on local machine

**#sudo apt-get update**

**#sudo apt install git -y**

To check version 

**#git version**

To check whether directory is part of git control system 

**#git status**

If it is showing that it is not under git then use git init. This will create a file as .git.

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/b005519d-2071-4754-84ed-bd376904ea5e)


**#git init**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/c62c4b2a-d0ca-4938-8991-d4d8f61b712d)

To add file from untracked to Staging use

**#git add filename**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/48e72c68-92cd-45fd-b24a-eb0186487638)

To remove any file any from staging to untrack use below command.

**#git rm --cached filename**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/b62b5fa9-8ee4-4b2a-8f9a-ce1a6489ec4a)

If you want to add to VCS or Track then use below command. if you are not to mention any auther then it will use hostname of your local machine.

**#git commit -m "added new file"**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/bdfe207e-e50e-4b87-83ac-99beb14f7c07)


If you get any error like set your isentity then use below command. Then try git commit

**#git config --global user.name "Firstname Lastname"**

**#git config --global user.email "your_email@youremail.com"**

If you deleted any file from this filesystem then how to restore. First check the status then you wil get to know whicjh file was deleted.

**#git restore filename**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/cd38d308-e3bc-4cef-a774-e89891c5b87d)






