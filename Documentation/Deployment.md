# Prerequisites
- [Node](https://nodejs.org/en/download/current/)
- [.Net](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)
- [Visual Studio](https://visualstudio.microsoft.com/downloads/)

# File Structure
```
.gitnore // git file to ignore files
TransactIQ.sln // The solution file that use loaded into visual studio
back-end
  |
  └─
front-end
  |
  └─ src
  |   |
  |   └─ assets // Folder for your static assets like images of fonts
  |   |
  |   └─ components // Folder that holds all of your components which are pretty much collections of js,html,css
  |   |
  |   └─ Main.ts // Where your app is loaded 
  |
  └─ package.json // This stores all the node package information
  |
  └─ vue.config.js // This stores all the vue basic config like port, proxy, certificates
  |
  |...
```

# Testing 
1. Clone repo 
2. open the TransactIQ.sln file with Visual Studio
3. Inside Visual Studio right click back-end in the solution explore then scroll down to "Set as Startup Project" and click
4. In VIsual Studio click the play button on the top navigation bar 
5. Open a windows command prompt 
6. cd into the front-end directory 
7. run npm install
8. run npm run serve
9. navigate to the website put in console
10. Insert [this file](https://github.com/Jake-R-Freestone/transactiq/files/9975772/ArchiveTransactionHistory_GoldSample.xlsx) where it says choose file.
11. If a table shows up you know you did it correctly. 
