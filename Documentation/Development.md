# How to replicate the development enviroment



## Requirements 

* Visual Studio
  * Under workloads - ASP.NET and web development
  * Under individual components - ML.NET Model Builder
* BitBucket
* Git
* Docker Desktop
* Yarn
* C:\Program Files\Git\bin in system path variables
* Accutech SSO account to log-in



## Steps

### Setup

1. Clone from the repo
1. Open ***TransactIQ.sln*** in Visual Studio
1. Right click the ***docker-compose*** and select ***Set as Startup project***
1. Ensure ***Docker Desktop*** is running
1. In ***docker-compose.override.yml*** paste in the Client Secret
1. In ***/src/backend/appsettings.json*** paste in ConnectionString
1. In ***/src/frontendVue*** directory run ```yarn```
1. Open ***Powershell*** as Admin
1. In ***/src/devHTTPS*** directory run ```.\Create-Certs.ps1```
1. In ***Visual Studio*** we can now run ***docker-compose*** by hitting the green start button

## Linting


## Tech Stack

* Docker

* frontendVue
  * Vue3
  * Vite
  * Yarn

* frontendServer
  * Duende
  * Proxy-server

* backend
  * ASP.NET Core Web API
  * PostgreSQL
    * AWS RDN
  * Swagger

## Folder Structure

```
TransactIQ
│   README.md
│       
│
└─── backend
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
|
└─── backend.Tests            # Tests for the backend
|
|
└─── frontendServer         # proxy server handles SSO and caching
|
|
└─── frontendVue
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


* src/backend/appsettings.json
  * This is where the ConnectionString is
* src/docker-compose.override.yml
  * This is where the Client Secret is

## Repo

https://github.com/Jake-R-Freestone/transactiq
