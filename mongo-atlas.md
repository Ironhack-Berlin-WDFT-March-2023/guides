#  MongoDB Atlas Setup 

### 1. [Signup for a free MongoDB Atlas account](https://www.mongodb.com/cloud/atlas/lp/try2)

![](https://i.imgur.com/vKJgkEB.png)

<br>

![](https://i.imgur.com/jLhyP7k.png)

<br>

### 2. [Signup and create a free cluster](https://docs.atlas.mongodb.com/tutorial/deploy-free-tier-cluster/)

1. Sign Up for Mongo Atlas: Enter email, password, first name, last name

2. Select **Starter Clusters (or Shared Clusters)** 

3. In the drop-down **Cloud Provider & Region** select: 

   -  Europe Region 

4. In the drop-down "**Cluster Tier**" select:

   -  **M0 Sandbox** - with the flag **Free forever**.

5. Click the button **Create Cluster**

<br>

![](https://i.imgur.com/uxoAE6C.png)

<br>

![](https://i.imgur.com/auYMuhb.png)

<br>

![](https://i.imgur.com/sOOp0vs.png)

<br>

![](https://i.imgur.com/j8kcopJ.png)

<br>

## 3. Setup MongoDB Atlas Cluster:

1. In the sidebar in the **SECURITY** part:

   - select **->  Database Access**

   <br>

2. Click on **<u>+ ADD NEW USER</u>** to create a new user

   - Select **Read and write to any database** - User Privileges
   - Set the **Username** and **Password**
   - Set **Database User Privileges** to : ***Atlas admin***
   - Create New User

   <br>

   ![](https://i.imgur.com/L9Pie5j.png)

   <br>

3. In the sidebar select **SECURITY  ->  Network Access**

   <br>

![](https://i.imgur.com/88GeH9u.png)

<br>

4. Click on **<u>+ ADD IP ADDRESS</u>**

- Click on **ALLOW ACCESS FROM ANYWHERE**

- Confirm

<br>

![](https://i.imgur.com/f3tGfbn.png)

<br>

5. Connect To Your Cluster: Click on the gray button **CONNECT**

- Select **Connect Your Application** option
- Choose Your driver version:  **DRIVER**: Node.js
- **Copy** the **Connection String Only**

<br>

![](https://i.imgur.com/btWKcLp.png)

<br>

![](https://i.imgur.com/7pYGh0P.png)

<br>

6. Update the connection string and add the ***username*** and ***password***.

<br>
