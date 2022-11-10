# Prerequisites
- [Node](https://nodejs.org/en/download/current/)
- [.Net](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)

# How to deploy
- Deployment has only been tested on windows but could work on linux
- Put folder with git clone anywhere
- To start the **back-end** system navigate to ***/back-end/bin/Release/net6.0*** and start ***back-end.exe***
- To start the **front-end** system in windows command prompt ```cd``` into the front-end directory, run ```npm install``` and ```npm run server```
- Servers should now be running 

# Errors 
- Errors will be logged into the command prompts running each part of the app.
- A common error is the back-end not communicating with the front-end. If this happens make sure you waited long enough for the back-end to boot up.
