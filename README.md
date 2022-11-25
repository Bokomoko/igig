# Sample MongoDB connection

This exercize intends to show how to connect a Node.JS program to the MondoDB Atlas Cloud NoSQL server.

This repo is for educational purposes only and can be used by anyone

## Contents

* .env.sample -> File with the environment variables used by the exercize. The .env.sample should be used as a template for the real life .env file that will indeed store the values.
* .gitignore -> This file will list the files and/or folders that will be uploaded to Github. The idea is to prevent uploading the libraries and package as well as the final compiled/distributed code. The .env file is added to the list to prevent the upload of critical information to the Github, like username and passwords
* .nvmrc -> This file contains the version of Node.JS used in this exercize. It's used by nvm, a tool that allows many different Node.JS versions to coexist in the same machine. We're using version 16.17.1. If your computer just have this version installed, you don't need nvm. If you plan to use other versions of Node in your computer, I strongly recomend to add the nvm tool.
* package.json -> This file contains the list of dependencies, ie, the libraries and packages that are used in this exercize. The package.json file also contains configurations for running on development environemnt, how to run it on production environment, how to test it, how to deploy it
* package-lock.json -> This file contains the instant snapshot of the last packages installed on the current version of the application

All the files mentioned above are very common in JavaScript projects.

* hospital.json -> is a sample of a "document" stored in the database. The idea here is to keep it simple and don't use the schema functionality. MondoDB allows for a very strict schema verification. We're not using it on this exercize since it's very introductory.
* index.js -> the very first and simple program to demonstrate how to connect and query a MongoDB database using JavaScript (Node)

### To run this project

First clone the repository to your local machine either using the command line git clone command or by cloning it inside Visual Code (or your preffered IDE)

After obtaining your local copy, create a .env file from the .env.sample. Fill it with the real credentials (username/password) and host information

Now it's time to install the dependencies. The dependencies are listed inside the package.json file. The following command will read the package.json file and install all the dependencies.

```bash
npm install
```

This will install all the packages that this project needs

After installing the dependencies ...

```bash
npm start
```
