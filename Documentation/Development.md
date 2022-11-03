# How to replicate the development enviroment



## Requirements 

* Visual Studio
  * Under workloads - ASP.NET and web development
  * Under individual components - ML.NET Model Builder
* BitBucket
* Git


## Steps

### Settup

1. Clone from the repo
1. Open the ***TransactIQ*** Solution in Visual Studio
1. Right click the ***/back-end*** directory and select ***Set as Startup project***
1. Right click the **/front-end** directory and select ***Open in Terminal***
1. In the Terminal, run ***npm install*** to install the required node packages

### Running the enviroment

1. In the ***/front-end*** directory run ***npm run serve*** to run the front end. You can open the front end in a browser ***https://localhost:5002***
1. After selecting the ***/back-end*** as the Startup Project, you can just hit the run button at the top of Visual Studio


## Tech Aspect

* Font-end
  * Standalone Typescript Vue Project
    * VUE3
    * Typescript
  * css

* Back-end
  * ASP.NET Core Web API
  * PostgreSQL


## Folder Structure

```
TransactIQ
│   README.md
│       
│
└─── back-end
│   │
│   └─── Models               # Models represent tables in the database
│   │   UserModel.cs
│   │   ...
│   │
│   └─── Controllers          # Provides routing and Model Queries
│   │     │   UserController.cs
│   │     │...
│   │     
│   └─── Migrations           # Database backups and Model states
|         │...
│   
└─── front-end
    │
    └─── src
          │
          └─── components      # Components that make up the pages
          |  Login.vue
          |  Table.vue
          |  Sidebar.vue
          │
          └─── assets          # Assets such as images
          |  logo.png
          |  ...
```


## Config Files

*There are not many config files that should be changed*

* If you need to change the port the app runs on
  * /back-end/Properties/launchSettings.json
  * /front-end/vue.config.js

## Repo

https://github.com/Jake-R-Freestone/transactiq
