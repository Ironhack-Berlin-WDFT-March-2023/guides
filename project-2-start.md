# Project 2 Start

### Setup repository on GitHub

One team member creates the repository on GitHub either in their **personal account** or as an **organization**.  
Add your other teammembers as collaborators:  
Settings -> Manage access

### Setup the project with Ironlauncher

Use Ironlauncher to create the basic structure for your project:  
```bash
$ npx ironlauncher@latest <ProjectName>
```
Choose: `views` and `no authorization`  

If Ironlauncher is installed globally:
```bash
$ ironlauncher <ProjectName>
```

### Push your project to GitHub

Push the created project to GitHub:
```bash
$ git init
$ git remote add origin <url to your repository> // Copy this line from GitHub after you created your repository
$ git add .
$ git commit -m "initial commit"
$ git push origin master
```

### Collaborate with other team members

Your other teammembers can now clone the project from GitHub.  
They should **not** fork the project.
