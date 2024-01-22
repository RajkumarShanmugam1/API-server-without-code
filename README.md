# API-server-without-code

## How to easily create and host your own REST API without writing a single line of code ?
- We will see how to easily create your own REST API server to be accessible on the internet without coding and without the need of hosting it on any hosting provider.

### Important
- This concept is only used for `get` operation or `display` functionallity through githup.

### Requirements :
- Node.js
- Git
- Post Man

### Setup local environment :
- Create a new folder or project with the name `API-Server-Without-Code`.
- Open the command line on the new folder.
- Enter the following commands (Installing the Node.js)

  - ```shell
    npm init -y
    ```
      - This will create a package.json file inside your project.
        

  - ```sh
    npm install json-server
    ```
      - Create a new file with the name `.gitignore` with the entry for node_modules inside it so the node_modules folder will not be pushed to GitHub while pushing the code to the GitHub repository.
    
- Create a new file with the name `db.json`, inser the following content:
  ```json
    {
      "users": [
        {
          "id": 1,
          "name": "Rajkumar",
          "age": 22
        },
        {
          "name": "Shanmugam",
          "id": 2,
          "age": 50
        }
      ]
    }
  ```
  
- Open `package.json` file and add the scripts section inside it:
  ```
  "scripts": {
    "start": "json-server db.json"
  }
  ```

### Deploy on local :
- Now, start the application by running the `npm start` command from the command line.
- open http://localhost:3000/users or http://localhost:3000/Collection_Name
  ![image](https://github.com/RajkumarShanmugam1/API-server-without-code/assets/76644058/069e40fb-4df3-4f08-8a36-4a6701e30802)

### Deploy on githup:
- First create one repository on the githup.
- After push the folder into the correspond repository.
- https://my-json-server.typicode.com/GIT_USER_NAME/REPOSITORY_NAME
  - Eg : https://my-json-server.typicode.com/RajkumarShanmugam1/API-server-without-code
  ![image](https://github.com/RajkumarShanmugam1/API-server-without-code/assets/76644058/5edfdc97-49ed-477e-a311-d836b23f29ee)

