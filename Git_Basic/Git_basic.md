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

To List these details

**#git config --list**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/122516c9-01be-43db-a6b5-3d2ea85087d5)


If you deleted any file from this filesystem then how to restore. First check the status then you wil get to know whicjh file was deleted.

**#git restore filename**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/cd38d308-e3bc-4cef-a774-e89891c5b87d)

If you change any thing in file then just check status. It will be in **untracked**. Then you need to make it to staging. then Commit. Below are the commands.

**#git status**

**#git add filename**

**#git commit -m "new changes"**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/def367cf-2719-4f92-a653-39651b616321)


How to check difeerencec in file. Always differnces when it is in **untrack** mode. It will only work there.

**#docker diff filename**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/7dcdd88a-442e-4ecb-90ad-73e14ab24104)

If you dont want these changes then at **staged mode** first remove and make it to **untrack status**.

**#git status**

**#git rm filename**                       (Will remove and send it to Untrack)

**#git restore --staged filename**         (Will restore and sen it to staging)

**#git restore filename**                  (Will restore original file)


![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/4b7503a9-e544-4390-bcda-5f0a3c932e2c)


How to check whether how many Commits are performed.

**#git log**

![image](https://github.com/Khushang49/GIT-GITHUB/assets/95266353/2ea61e60-cebd-4fbf-a5ed-3d31f5a0ad21)

To copy any repo or any file from remote sercer. Always copy these folders in different directory where local repos are not there.

**#git clone giturl**


What is difference between git clone and git pull.

So whenever you want copy anything from Remote server to local server then we will use git clone. If we want to add any changes which is done on that Repo then we use **git pull** . We can use clone everytime.

If we want copy any repo from remote server to remote then use **git fork**



