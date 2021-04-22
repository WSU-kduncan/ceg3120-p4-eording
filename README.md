### Project 4 Documentation 


## Run Project Locally 

How to install docker - installed via the link provided. For WSL 2, I went into powershell and set default to WSL2. 
My command: wsl --set-version Ubuntu-18.04 2

How to build the container - docker build -t ceg:20 .

How to run the container - docker run -d -p 5000:80 ceg:20

How to view in browser: 127.0.0.1:5000
 
