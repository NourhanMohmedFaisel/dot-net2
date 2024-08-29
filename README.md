# Create a new project on your local machine, then push it your remote repo.

     git config --global user.name "NourhanMohmedFaisel"
     git config --global user.email "mnourhan527@gmail.com"
     git init
     git add .
     git commit -m "commit number one"
     git remote add origin git@github.com:NourhanMohmedFaisel/dot-net2.git
     git push origin master

# Create two branches (dev & test) then create one file on each branch, and push this changes to the remote repo.

    git checkout -b dev
    git add dev.html
    git commit -m "commit dev branch"
    git push origin dev

    git checkout -b test
    git add test.html
    git commit -m "commit test branch"
    git push origin test

# Merge this changes on Main branch and then push it to your remote main branch

    git checkout master
    git rebase dev
    git rebase test
    git push origin master

# Tell me how to remove them locally and remotely.

      git branch -d BranchName ====> delete locally

      git push origin : BranchName  =====> delete remotely

# Tell me how to checkout another branch without commit changes

      git stash

      git checkout BranchName

# Create an annotated tag with tagname (v1.7) & push it in remote repository

      git tag -a v1.7 -m "version1.7"
      git push origin v1.

# Tell me how to list tags.

     git tag

# Tell me how to delete tag locally and remotely

            git tag -d TagName ====> locally

             git push origin : TagName ====> remotly

<img src="moon.jpg" alt="moon">
