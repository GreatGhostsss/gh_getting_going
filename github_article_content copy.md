This is for GitHub users who want to translate their knowledge of working with the GUI version of GitHub to the command line. 

Let’s say you’re green, but not that green. Let’s say you want to learn more about GitHub, but can only find tutorials for either brand new users or advanced workflows for GitHub vets—nothing in between. 

This is where this page comes in.

---------------

Stay with me for a minute. 

This is essentially a getting started guide. And there are naming conventions when it comes to documentation like this. If you're new, we have Getting Started. If you're an experienced user, we have the imperfect convention of 'Advanced [thing] in [tool or language].' What about between getting started and advanced concepts? Maybe we could have a learning more about. But what's between Getting Started and Medium. Getting Medium? 

Yes, we're getting medium.

----------------

### Assumptions

- You're familiar with the GUI version of GitHub, GitHub Desktop
- You want to be more comfortable with the command line
- You’re somewhat familiar with concepts that sound weirdly like throwing a frisbee with your dog: push, pull, fetch

-------------------

### Scenario One:  Place the files hosted in your GitHub repository onto your local machine 

We want to take an already-existing repository and place it on your local machine. The good news is that you'll only have to do this once. 

$ git clone http://yourproject.com/coolRepo.git

This command deposits a clone of repository in the /Users/ directory on your Mac

### Scenario Two: Update local repository to match what's on the server

This scenario is relevant if you’ve made a change to one of your files in GitHub itself and want to ensure you’re working locally with the most recent copy. This is rare, but good to know how to do. 

1. In your browser, visit the GitRepo to which you want to push. 
2. Click **Clone or download**.
3. Copy the URL. 
4. In Terminal, pull from the repository using this command, replacing my sample URL with the URL copied in step three.

$ git pull http://yourproject.com/coolRepo.git

Pull/Fetch/the difference between the two

You have to CD to the folder you’re fetching/pulling from

###Scenario Three: Push changes to repository 

You’ve made changes in your local environment and want to ensure your GH repo reflects them. This is the most common scenario. 

For context about why we're doing what we're doing, we need to understand what the staging area is. 

The staging area is a magical, liminal space where changes you've commited hang in the air, waiting for you to gently glide, er, push them into your repository. 

After making changes to a file locally, we want to place that file in the staging area. We can do this with $git add [file], but git commit -a -m "" is comprehensive and easier to use. 

We can ensure the changes we've placed in the staging areas are recognized by Git using $ git status. If the file name is green, Git has recognized the change and is ready for you to push to the remote repository.

To push to the repository, we only need $ git push

For the last, and arguable most important step, the syntax for this command is straightforward.   

[META]

Choices re: an imperative style vs. "we": I prefer the latter when writing content whose nature can be intimidating. The plural voice mimicks a hand-holding style of process oriented writing that I personally find helpful. 

[META]

I deliberately used the inanimiate whose in the above paragraph. 

I have not used "simply."