# Prerequisites
- [Node](https://nodejs.org/en/download/current/)
- [.Net](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)

# How to deploy
- Deployment has only been tested on windows but MAY work on linux
- Put folder with git clone anywhere

## To _start_ the **back-end** system
Navigate to ***/back-end/bin/Release/net6.0*** and start ***back-end.exe***
## To _start_ the **front-end** system
In windows command prompt ```cd``` into the front-end directory, type ```npm install```, then ```npm run server```
- Both servers should now be ready and running

## To _stop_
Simply close out of both front-end an back-end browser windows

- Troubleshooting:
    * If trying to run browser for front-end with localhost:5002 and receive 'Cannot connect' error message, go back to front-end directory and type ```npm run server``` to make sure server is running and try again

# Errors 
- Errors will be logged into the command prompts running each part of the app
- A common error is the back-end not communicating with the front-end. If this happens, make sure you waited long enough for the back-end to boot up
