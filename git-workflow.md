# Git-Workflow

## Resources

- Git Cheatsheet by GitHub: https://education.github.com/git-cheat-sheet-education.pdf
- Git Tutorial: http://gitimmersion.com/

## Process

Checkout main branch: 
    
    git checkout main

Create a new branch and checkout branch: 
    
    git checkout -b <branch-name>

Work on your feature and then add the files and commit them: 
    
    git add .
    git commit -m "commit message"

Push to remote repository. If the branch does not exist on GitHub it is created: 
    
    git push origin <branch-name>

Open github repository and click on "New Pull Request"  
Review pull request and merge it to main

Pull changes from GitHub repository to your local branch:
    
    git checkout main
    git pull origin main

Delete feature branch after feature is merged:

    git branch -d <branch-name>
