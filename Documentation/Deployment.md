# Prerequisites
- [Node](https://nodejs.org/en/download/current/)
- [.Net](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)
- [Visual Studio](https://visualstudio.microsoft.com/vs/community/)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [WSL](https://learn.microsoft.com/en-us/windows/wsl/install)

# To replicate
1. Open Docker Desktop
2. Clone poject
3. Open powershell
4. navigate to {projectDirectory}/scr/DevHttps
5. Run Create-Certs.ps1
6. Run docker-compose  -f "docker-compose.yml" -f "docker-compose.override.yml" -f "obj\Docker\docker-compose.vs.debug.g.yml" -f "docker-compose.vs.debug.yml" -p dockercompose10224266510018579893 --ansi never up -d

# How to deploy
- Deployment has only been tested on windows but MAY work on linux
- Put folder with git clone anywhere

## To _stop_
Stop the process on docker desktop

## Troubleshooting:
 If trying to run browser for front-end with localhost:5002 and receive 'Cannot connect' error message, go back to front-end directory and type ```npm run server``` to make sure server is running and try again

# Errors 
- Errors will be logged into the command prompts running each part of the app
- A common error is the back-end not communicating with the front-end. If this happens, make sure you waited long enough for the back-end to boot up
