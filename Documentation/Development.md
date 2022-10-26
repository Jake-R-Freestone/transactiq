# How to replicate the development enviroment



## Requirements 

* Visual Studio
  * Under workloads - ASP.NET and web development
  * Under individual components - ML.NET Model Builder
* BitBucket
* Git


## Steps

1. Clone from the repo
2. Open in Visual Studio
3. Right click the *TransactIQ Solution* in Visual Studio Solution Explorer and select *Properties*
4. Expand *Common Properties* and select *Multiple startup projects*
5. Ensure that *back-end* is set to Start before *front-end*
6. Click start or press *ctrl+F5*

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
