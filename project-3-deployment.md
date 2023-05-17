# Backend deployment on Cyclic

## Project structure

Your project should consist of two GitHub repositories:  
- server  
- client

## MongoDB Atlas

If MongoDB Atlas (Cloud MongoDB, not local MongoDB) is not set up:  
Follow the steps in the guide `project-2-start` to setup MongoDB Atlas.

If you want to create a new Cluster on MongoDB Atlas you have to create a new project:  
https://docs.atlas.mongodb.com/tutorial/manage-projects/#create-a-project

## CORS setup

Configure CORS in config/index.js:
```js
const FRONTEND_URL = process.env.ORIGIN

app.use(
  cors({
    origin: [FRONTEND_URL]
  })
)
```

## Deployment on Cyclic

1. Open https://www.cyclic.sh/

2. Click on **Sign Up**

3. Click on **Continue with GitHub**

4. Submit

5. Under **Deploy your first app** click on **Link Your Own**

6. Search for your **server**-repository  
(Please be aware: You cannot deploy from an organization)

7. Click on **connect**

8. You can find the link to your deployed application under **api deployed at**

9. Open **project dashboard**

10. Under **variables**, add environment variables from .env  
(Don't forget to add ORIGIN after you deployed the client)

11. Under **environments**, you can customize the url for your app

# Frontend deployment on Netlify

## Configure API_URL

Create a .env-file to configure your API_URL:
- Create a .env-file in the root-level of your client-repository  
- Add a variable `REACT_APP_API_URL=<server-app-URL>`  
- Replace the `API_URL` in all axios-requests with the REACT_APP_API_URL from the .env-file: `process.env.REACT_APP_API_URL`

## Deployment on Netlify

- Add a file named `_redirects` in your public folder with this content:
```
/* /index.html   200
```

- Follow the instructions in the student portal: `React | Deployment on Netlify`  
- Add the environment-variable REACT_APP_API_URL

If you have problems with the build-process after the deployment, you can also manually build the app and deploy it:
- Add the `server-url` as REACT_APP_API_URL in the .env-file  
- Run `npm run build` in your client-repository to create the static files  
- Choose `deploy manually` on Netlify and drag or browse to the just created build-folder inside your client-repository

And... that's it! Happy deployment 🚀
