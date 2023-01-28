# ELI5 - Git: The Version Control System(VCS)

# What is git?

Git is an open-source version control system. Now, you might be thinking what the heck this means... but don't worry, I will explain to you every single word that I have written like I am explaining to a 5-year-old.  
\- Git is just a name that has been given to this version control system, which is an open-source software maintained by some amazing developers.

\- Version Control System is a system that has been developed to manage, maintain and to be in sync with your collegues and other collaborators who are working on the same project.

\- There are projects, software, applications, etc being built, by some developers and their source code is made available to the public so that developers around the world can see, go through the code, fix the existing issues and contribute to the code base in order to maintain and improve the software. This is what exactly open source software means.

# Why VCS?

Imagine a scenario, where you and two of your other friends are working from home because of covid, on a project that needs to be build with multiple features in it. Now, think of all the ideas by which you can collaborate with each other. If you think of sending the finished project files via email, then the attachments can be too large. If you think of doublt-tripple compression, even then the file will be too large and another hassle to decompress the file multiple time comes to the picture. If you think that you will upload the files to gdrive or something like that then there can be big conflicts in the file structure and can result in breaking the appli,cation.  
So, exactly for this reason, the version control system aka VCS was developed.

The VCS helps teams solve these kinds of problems. It tracks every individual changes by each and every contributor, helps in preventing conflicts. It basically takes a snapshot of all the work you have done so far. Each of the contributors can work on their feature independently and merge everything into one after they are done with their work on the project.

# How to use git?

To use git, like every software, we need to download and install git on our systems and where do we download and install git from? We download and install git from [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

# What after installing git?

* After installing git, open your [terminal](https://www.ionos.com/help/email/troubleshooting-mail-basicmail-business/access-the-command-prompt-or-terminal/) and type:
    

```bash
git --version
```

This will show you the currently installed version of git.

* To work with git or in other words, in order for git to track all the changes in the project, you need to ask git to do that for you and how do you ask git to track your project? You simply type:
    

```bash
git init
```

This command will initialize an empty git repository for you. Basically this means that git will now start to track all the changes made in your project.

* Git will also tell you the status of all the tracked and untracked files when you type:
    

```bash
git status
```

* For git to add the files to it's tracking list, you will need to add the files manually by using the command:
    

```bash
git add file_name
# if you want to add all the files to the tracking list, then use the command:
git add .
```

* After adding the files to the tracking list, you will need to cofirm that you want to make the changes permanent by commiting that change in the tracking list by using the command:
    

```bash
git commit -m 'commit-msg'
```

* If you want to work on a differnt feature of the project that you are building and work in a way that the changes you make in your code does not change anything in the final code until you are satisfied with your work then you can create different branches by using the command:
    

```bash
git branch branch-name
```

* You can create multiple branches and work on multiple feature independently of other features by creating multiple branches.
    
* To get an overview of all the branches you or your team mates have created so far you can use the command:
    

```bash
git branch
```

* To switch between various created branches you can use the command:
    

```bash
git checkout branch-name
```

* To combine the work you and your friends have done you can use the command:
    

```bash
git merge branch-name
```

* To send your changes to the production, you will need to push your code to your repository by using the command:
    

```bash
git push remote-repository branch-name
```

* If you want to check history of everything that has happened to a git repository then you can use the command:
    

```bash
git log
```

* Now what is this production and repository?
    
    * Production is the final environment in a software developement process. When a code is pushed to production then it means that all the changes made in the code is finally available for the public to use.
        
    * Repository is the collection of file and folder structure containing all the different versions of a project.
        
* If you have to collaborate on some existing projects that is already being worked upon, then you will need to pull the code from you github or gitlab account by using this command:
    

```bash
git pull remote-repository-url
```

* What is a remote repository?
    
    * A remote repository is a repository that is not on your local system but at a remote location like github or gitlab.
        
* What is github and gitlab?
    
    * Github, gitlab and there are other services also. These are the companies that offer cloud based git repository hosting service which makes it easier to collaborate on any project.
        

This is all the information that was required to understand the version control system - git. I have covered all the basic and most used commands that we use in our day to day life as a software developer. I tried to explain everything in a way as if I was explaining to a 5 year old.

Drop down your comments, suggestions or something important that I missed on. I will try to cover it up on my next blog.

If you want to get in touch with me or know more about me then just google "clevercoderjoy".