## Learn Git and Github. (Part - 1)

### Basic Intro : 
**Suppose you are painting a scenery for your school competition. You finished the painting and at present you are adding some final touch to it. Now, let us suppose you tried to mix some colors and your painting suddenly loses it's charisma. You commited a mistake. Now you badly want to revert back to your last drawing,(the drawing you had before mixing the colors). How will you do this? This is where our Protagonist for the blog "Git" comes into action.**

### What is Git?
**If we go by the definition on Git's official webpage :  "*Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency*."**

**That is big definition for a beginner. "Distributed Version Control System", is a big term for newbies. Remember the example at the start of the blog? Every time you modify your painting, the modification gets stored by a software in a proper order. So now suppose you draw a tree in your painting but after drawing you see that it is not looking good, with the help of Git you can revert back to the painting you had before you drew the tree.**

**That is what is Version Control. Easy? Now obviously Git cannot be implemented in your drawing, so paint your painting carefully! :) **

**For Software Developers, Git is an awesome tool. It tracks all the changes and it has way more functionalities than that.
**

**For Folks into Open Source, this is the link for git's github repository -> https://github.com/git/git**

### So what is Github?
**Github is a service. It is a cloud hosting service used to manage your Git repositories. You do not need Github to use Git. But the opposite is not true. You need Git in your system to use Github. Following our example :  Your painting is now hosted on a cloud platform and all your commits(modifications) are stored on the cloud in addition to your local device. Everybody can see your painting and all the new commits you add to it.**

**What is a repository?  It is just a term for a folder which contains everything related to your project. It also contains all the files related to your commits, license, README, etc.
We will go in depth of a repository and how to create one in Github in the next part of the blog. 
**

## Tutorial Section : 

### 1. How to install Git -> 
**Step 1 : **Search install Git on your browser or click on this link : https://git-scm.com/downloads

**Step 2 :** Click on Download on basis of your OS. For Windows user, Click on the link as shown in the picture below.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656183583540/z11mWrAVM.png align="left")

**Step 3 :** Now just keep on Clicking next until the following page opens, as shown below. Just tick those two options as shown.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656183767138/k7VnBzDba.png align="left")

**Step 4 :** Continue clicking next and at last click on Finish. 

**Step 5 : **This should install Git successfully in your system. 

### 2. Creating our first Repository -> 

**Step 1 :** Create a folder. We have created a folder named "Git Tutorial". Open the folder, right click and you will see an option as Git Bash. On clicking it, a terminal will open.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656184184592/7U94Rpyxo.png align="left")

**Step 2 :** Once the terminal opens, you are ready to write your first Git Command. Step ahead and write "git --version" and press enter. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656184364591/RN2yyxHLy.png align="left")

Congratulations! You have not only installed Git successfully in your system, but also you have written you first Git Command Line Argument. 

**Pro Tip : **Open the Terminal infront of your non-programmer friends and then let them think you are a hacker! :)

**Step 3 :** Now let us configure your username and email. For this, follow the screenshot below. Enter your name, and your email id as shown below.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656188108016/ypccQD5gI.png align="left")

After entering you can use the command "git config --list" to see your name and email.

**Step 4 :** Now let us create a repo(short for repository). In the terminal type "git init". This command initializes an empty git repository.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656184626193/MeaRq8892.png align="left")

**Step 5 :** Now all git functionalities can be performed in this folder, or rather you can now call it a Repository. We will learn about how to create a file, make changes, revert changes, etc in a short while.

### 3. Some Common Git Commands

**1. **"*git*" -> Shows the common git commands. You can also type this to check whether you have successfully installed git in your system or not.

**2.** "*ls*" -> It is the list command. This lists all the files in your folder/repo.

**3.** "*mkdir {name of folder}*" -> This is the Make Directory Command. Creates a new folder.

**4.** "*cd {name of folder}*" -> This is the Change Directory Command. It helps us to go inside a particular folder.

**5.** "*ls -a*" -> Shows all hidden folders.

### 4. Creating Files and Modifying them 

Now, we will see some examples on how to create files and modify them. This part is important because these are the most frequent commands that you will be using when you use Git on a daily basis. 

**Step 1 :** Creating a file. We use the command "touch {filename.type}" to create new files. This is shown below.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656185925550/AHwPjHShG.png align="left")

**Step 2 :** So we have made modifications to our folder. We have added a new file in our repo. To check the changes/the status of our repo, we type the command "git status". This is a very useful command and we use it very frequently. It is shown below.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656186102784/UPRww4ijv.png align="left")

**Step 3 :** Now you will see that is shows that 'you have untracked files'. Let us understand this with the help of our painting example. 

You want to document every commit you perform on your painting, thus you will need a scanner. You draw a tree. Now you put it in the scanner ready to be scanned. Then you press the button and the painting gets scanned. Your changes get saved.

In Git once we make some changes, we use the command "git add" to put the changed files in the staging area, to get ready to be documented and saved. This is like putting our painting in the scanner, just before it gets scanned. 
Now suppose you want to add something more to your painting and then scan it, you use the command "git rm --cached {filename.type}" to remove it from the scanner. You again apply some changes and then put it in the scanner. 
Now your painting is ready to be scanned and your changes are ready to be saved. Now we use the famous command "git commit -m {commit message}". Your changes are saved. You might have heard about the different versions of the software. This is it. Now you have a version of your painting. Ver 1. Again you can modify the painting and commit the changes and update it. Hope you have understood! Easy, right? :)

Let us see all these commands in action.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656187254376/bvyy_-9OC.png align="left")

### 5. Checking log, Deleting and Reverting changes

**Step 1 : **Suppose we want to check the history of all the commits that we have made. In this case, we can use the command "git log". This command will show us all the commits we have made.

**Step 2 :** If we want to delete a file we use the command "rm -rf {filename.type}".

These two commands are shown below.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656187636639/Nd-QvTWE0.png align="left")

**Step 3 : **Now, we have deleted the file. Let us now add and commit the changes. 

**Step 4 : **After commiting the changes, now let us try to revert our changes and bring back the file which we just deleted. Sounds cool? Let's do it.

We use the command "git reset #{id}". We will get the id from the log history. It is shown below. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656189680868/dBc9_bCuP.png align="left")

An Important point : When we use the command to reset, we use the id of that particular commit and all changes after that particular commit(from old to new) gets reverted. This is common sense. Otherwise you see, reverting only that particular commit will have catastrophic effects, and this is not what Version Control is about. So what does the reset command do? -> Undo all the changes after the id.

Let us bring back the deleted file now.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656189940057/1mfHGg563.png align="left")

We have used the command "git restore {filename.type}" to remove the file from staging area without committing.

Thus, we have succesfully completed a complete cycle from creating, saving, deleting and then again reverting to the original file. 

### 6. Some additional commands

**1.** "*vi {filename.type}*" -> This command allows us to edit within the file.

**2**. "*cat {filename.type}*" -> This command displays the file contents. 

One more thing that you might have noticed is this "master" tag. Wonder what is this? 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1656190672225/EGZ-nH4_V.png align="left")

This is what we call branches. Everything we did till now, was done on the master branch of our project. We can create many more branches which will ease our development process. We will learn more about branches in the next blog when we learn about Github. 

## Conclusion 

Although these were the most common and important commands to start your journey into Git and Github, what we have learned is mere basics, and there is always a lot more to learn. I hope you have understood what we discussed in this blog. See you in my next blog. :)


Connect with me : 

- [Twitter](https://twitter.com/sanjeeban_5644)
- [Github](https://github.com/sanjeeban5644)
- [Linkedin](https://www.linkedin.com/in/sanjeeban-mukhopadhyay-4bb4b01b8/)




