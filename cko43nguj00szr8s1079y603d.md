## How To Contribute To An Open Source Project On Github

Are you a Coder seeking an easy way to contribute to a project on GitHub? Yes!? then I have put up this article especially for you.

My name is [Grace](https://graceomowunmi.netlify.app) and I am a backend developer. If you are a Coder seeking how to contribute to a project on GitHub, or probably after reading my previous article on the [Benefits of Teamwork in Programming](https://gracious-grace.hashnode.dev/what-you-do-not-know-about-working-together-as-a-team-in-programming), you made up your mind to join a team but you are worried about how to use GitHub to always submit any task you will be assigned to do, do not worry, I am going to walk you through the **Fork-Clone-Contribute-Push-Pull request** path as simple and as precise as possible.

Let's begin.

### GITHUB
GitHub is a social platform that allows developers at different locations to collaborate. Git allows us to track all source code in a single location. If you are a complete novice about Git, GitHub, and its installation process, I will advise you to look into [this](https://www.google.com/amp/s/www.freecodecamp.org/news/the-beginners-guide-to-git-github/amp/) first 😊.

### PATH TO FOLLOW IN CONTRIBUTING TO A PROJECT
**FORK**-
To fork a project means to pick up the duplicate of that project's original repo from someone else's GitHub page to your own GitHub page. It is as simple as that. 

To fork a repo, follow the steps below:
- Navigate to the GitHub page of whose repo you want to fork.
- Click on the project/repo, on the top right of the page, you should see a button labeled "Fork". 

![fork.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619772819238/5zUe6QJR7.png)
- Click on this "Fork" button, follow the prompts, and select your account in which the forked repo will appear.
- Navigate to your own GitHub page and refresh. The forked repo will now appear as one of your repositories(don't be too happy) because it will be indicated as a "forked" repo(lol)😊

> 
Note: Repo is a short form of a repository.

**CLONE** - 
To clone a repo is to simply download that forked repository into the local environment of your computer so you can make changes.

To clone the forked repo, we will be walking through the following steps:
- Navigate to the forked repo and click on the big green button labeled "code".
- Copy the HTTPS URL by clicking on the button that has the copy image on it as indicated in the image below.

![clone.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619714196174/MHPfDUkQO.png)
- In your local environment, create a folder on your desktop or any other location of your choice. 
> 
I created mine on my desktop and named it "spoon_knife_sample".
- Open git CMD, make sure you are in your working directory(the folder which you created earlier), this is where we want the forked repo to be downloaded.
- Type in the following command to clone the repo, type "git clone https_url_that_we_copied_earlier" as indicated in the image below, sit back, and wait until it is downloaded.

![clonee.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619730580169/KUwRWlQlG.png)
**CONTRIBUTE** - 
Now that you have the repository on your local machine, open the folder with your text editor(I use Visual Studio Code), play around with the codes, make changes, add new features, and get it ready to be pushed back to where it came from(GitHub)😊. We are approaching our destination gradually(lol).

**PUSH** - 
To push a repository is to push a local repository from your computer to a remote repo(the repo on GitHub).

To do this,
- Open your Git CMD.
- Navigate to your working directory.

> 
Note: You do not need to "git init" again, because git has already been initialized after you cloned the repo.

Type in the following commands in wrapped in quotation mark:
- **"git status"** - 
This will show the modifications you have made in the folder or the new(untracked) files you have added.

![commit.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619712803818/MopV8FlD6.png)

> 
Note: The word "main" that I underlined could be either  "main" or "master".

- **"git add . "** - 
![add.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619712819994/es8-BC3RW.png)
This will add all the modified and new files to the staging area.

- **"git commit -m "your commit message"**  " -
The git commit command is used to save changes to a local repository after staging it, while the commit message should indicate or state the changes you have made for easy reference.
- **"git remote -v"** - 
This makes sure you are pushing to the right upstream(your forked repo).

- **"git push origin main"** or **"git push origin master"** - Depending on the name of the branch following how I explained earlier(could be "main" or "master". Now, your local repo has been pushed to the remote repo on your GitHub page.

**The whole push process**👇

```

C:\Users\grace_omowunmi>cd desktop

C:\Users\grace_omowunmi\Desktop>cd spoon_knife_sample

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample>cd Spoon-Knife

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    contact.html
        modified:   styles.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        info.html

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>git add .

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>git commit -m "deleted contact page, modifies page styling and added info page"
[main 0233288] deleted contact page, modifies page styling and added info page
 2 files changed, 1 insertion(+), 1 deletion(-)
 rename contact.html => info.html (100%)

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>git remote -v
origin  https://github.com/gra2101/Spoon-Knife.git (fetch)
origin  https://github.com/gra2101/Spoon-Knife.git (push)

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>git push origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 1015 bytes | 169.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/gra2101/Spoon-Knife.git
   934d096..0233288  main -> main

C:\Users\grace_omowunmi\Desktop\spoon_knife_sample\Spoon-Knife>
``` 

**PULL REQUEST** - 
A pull request is a way of submitting contributions to an open-source project. Pull request occurs when a developer asks for changes committed to an external repository to be considered for inclusion in a project's main repository. To pull request,
- Return to your GitHub page and refresh, you will see your recent commit.
- Click on the button labeled "pull request", 

![pullrequest.PNG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619714479648/WHbXn7m_w.png)
- On the next page you will be redirected to, add a "read me" file clearing stating the content of the branch or the changes you have made.
- Click on create pull request. 
Tada!! We have gotten to our destination😊.

Now, sit back, fingers crossed, if your pull request is accepted, the coordinator will merge your branch into the head branch and then it becomes a single project.

Congratulations!!! You have successfully contributed to a project.

I hope this helps! Bye👋...

 










