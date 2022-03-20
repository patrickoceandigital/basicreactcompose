- Basic application in REACT using one variable in .env file

build basic image
- docker build -t reactapp .  

run image with default value
docker run -p 3000:3000 -t reactapp

run image with overidden value from run command of docker
docker run -p 3000:3000 -e REACT_APP_API_URL=google.com -t reactapp

run image with overriden value from run of docker-compose basic using file definition
docker-compose up



WARNING: env_file: section will be overridden by environment:
    env_file:     
    - .envcompose
    environment:    #comment this if you want to env_file to be used
    - REACT_APP_API_URL=netflix.com