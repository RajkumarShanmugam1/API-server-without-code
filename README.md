# API-server-without-code

## How to easily create and host your own REST API without writing a single line of code ?
- We will see how to easily create your own REST API server to be accessible on the internet without coding and without the need of hosting it on any hosting provider.

### Important :
- This concept is only used for `get` operation or `display` functionallity.

### Requirements :
- Node.js
- Git

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

- Now, start the application by running the npm start command from the command line.
- http://localhost:3000/user
