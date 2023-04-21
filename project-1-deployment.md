# Project 1 Deployment

## Create the local project

Create the project folder:  

```bash
$ mkdir <name of the project>
```

Work on your project  

Commit your changes:  

```bash
$ git init
$ git add .
$ git commit -m "Initial commit"
```

## Create the repository on GitHub and connect it to your local project

Create a new repository on GitHub and add it as a remote repository:  

```bash
$ git remote add origin <url to the repository>.git
$ git push origin main
```

## Deploy your app to GitHub Pages

Follow the steps in this guide to deploy your app to GitHub Pages:  

https://docs.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

### TLDR

* Navigate to the GitHub repository you want to deploy

* Click on **Settings**

* Under **Pages**, click on **None** and select the main (or master) branch as publishing source

* Click **Save**

* After a few minutes you will see the URL of your deployed app

* You only need to do this once: Whenever you push to master, the app is automatically updated
