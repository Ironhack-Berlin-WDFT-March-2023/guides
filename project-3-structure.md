### First use Ironlauncher to start the project and create the backend - we will use the json flag to create a json api template.

### In this example our project will be called 'projector'

### Select "No auth"

```bash
$ npx ironlauncher@latest projector-server --json
```

### To create the client we will use create-react-app
```bash
$ npx create-react-app projector-client
```

### This should result in the same structure that we have [in this example](https://github.com/Ironhack-Berlin-WDFT-January-2023/w8d1)

### Then we can connect both repos to github and make the first commit

```bash
$ git add .
$ git commit -m 'initial commit'
git push origin master/main
```

Now we have our basic project structure 💪 

The other team members can now clone the repos from GitHub (make sure to run npm install in both the server and in the client folder).

Happy hacking 💙