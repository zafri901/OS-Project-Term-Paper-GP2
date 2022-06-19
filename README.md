# OS Project Term Paper GP2

TUTORIAL ON DOCKER SYSTEM MONGO DATABASE

Prepared By : 

| NAME  | MATRIC NO. |
| ------------- | ------------- |
| MUHAMMAD NOR ZAFRI BIN AHMAD  | 1913139  |
| MUHAMMAD FARIS BIN MUSA  | 2013259  |
| MUHAMMAD ALI ASGHAR BIN MUHAMMAD NASIR  | 1918589  |

# CONTENT

1. Introduction
2. Steps and procedures of installation
3. Installation of Docker
4. Installation of WSL 2
5. Installation of MongoDB
6. Examples of code and commands
7. Sample run MongoDB

# Introduction

Docker is an open source software platform to create, deploy and manage virtualized application containers on a common operating system (OS), with an ecosystem of allied tools. Docker container technology debuted in 2013; Docker Inc. was formed to support a commercial edition of container management software and be the principal sponsor of an open source version. Mirantis acquired the Docker Enterprise business in November 2019.



# Steps and procedures of installation

## Installation of Docker

1. Download docker from the official website https://docs.docker.com/desktop/windows/install/
![1](https://user-images.githubusercontent.com/84853773/174477254-4105c004-0dbe-439c-bc8e-ec883099013e.png)
2. Run the installer and finish the installation
3. Open the application and finish the setup

## Installation of WSL 2

1. Download WSL 2 from Microsoft's official website here https://docs.microsoft.com/en-us/windows/wsl/install-manual
![11](https://user-images.githubusercontent.com/84853773/174477278-9bd8ab7f-8ac9-4928-bf58-46569004a7f2.png)
2. Run the installer and finish the istallation  
![13](https://user-images.githubusercontent.com/84853773/174477283-60f03df8-6330-4d75-bc5b-251e8970b1e4.png)

## Installation of MongoDB

1. Open Docker Desktop
2. Search for MongoDB at home page
3. Click the "Run" button to proceed the installation
![15](https://user-images.githubusercontent.com/84853773/174477288-4f794651-da10-494b-b7e1-8f8422756dda.png)
4. After completed the installation, open Windows Powershell
5. Type the “docker run -d -p 82:82 --name group-2-os mongo:latest” command inside the Powershell to create a container for the database.
![17](https://user-images.githubusercontent.com/84853773/174482307-ed20d3b5-f6d6-471f-aec6-272ee2e0ea14.png)
6. Closed the Win Powershell
7. Open the docker again and we will see the new container was created. Make sure we choose the correct container and open the terminal.
![18](https://user-images.githubusercontent.com/84853773/174477294-8e9ce0bf-ff1c-4bc2-a599-592332bd966f.png)
8. Type "mongosh" on the terminal and you are good to go

# Examples of code and commands

| Command  | Function |
| ------------- | ------------- |
| db.help  | To get a list of commands, type db.help() in MongoDB client. This will give you a list of commands as shown in the following screenshot.  |
| show dbs  | Use the command to get list of all databases.  |
| use DATABASE_NAME  | To create a new database execute the following command.  |
| db  | To know your current working/selected database execute the following command  |
| db.dropDatabase()  | To drop the database execute following command, this will drop the selected database  |
| db.createCollection(name)  | To create the new collection execute the following commands  |
| Show collections  | To get the list of collections created execute the following command  |
| db.COLLECTION_NAME.drop()  | To drop the selected collection execute the following command  |
| db.COLLECTION_NAME.insert(document)  | Insert document in collection  |
| db.COLLECTION_NAME.find()  | To get the list documents in collection execute the following command  |
| db.COLLECTION_NAME.update(SELECTION_CRITERIA, UPDATED_DATA)  | To update the document in collection execute the following command  |
| db.COLLECTION_NAME.save({_id:ObjectId(),NEW_DATA})  | To save document in collection execute the following command  |
| db.COLLECTION_NAME.remove(DELLETION_CRITTERIA)  | To delete document in selected collection execute the following command  |

# Sample run MongoDB

1. Type "mongosh" to start
![mongosh1](https://user-images.githubusercontent.com/84853773/174483109-e611681d-4b2c-43f9-b9fa-1c5c526c2ed9.png)
2. Type "use clinic" to enter clinic database. Create a new collection using "db.createCollection(name)" command
![mongosh2](https://user-images.githubusercontent.com/84853773/174483113-b1e537e8-8656-4b81-adf2-935641d14155.png)
3. By using db.instrumentone.insertMany() to enter the data into our database
![mongosh3](https://user-images.githubusercontent.com/84853773/174483115-b4bc5201-5255-4a1b-9b58-49a1125e6d1e.png)
4. View the database using "db.COLLECTION_NAME.find()" command
![Screenshot (198)](https://user-images.githubusercontent.com/84853773/174483117-0a195b2d-cbad-4485-9623-eba73382ac86.png)

