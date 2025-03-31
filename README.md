# docker-commands
### let's assume there is a image hello

// list containes
## docker ps  or docker container ls

// check what ps can offer
## docker ps  --help 

// run image
## docker run -d hello      

// remove containers
## docker rm        
## docker rm $(docker ps -aq)      
## docker rm -f $(docker ps -aq)      

// remove images
## docker rmi       

// pull images 
## docker pull hello
  
// bind port 
## docker run -d -p 8080:80 hello
// giving name to container
## docker run --name hello -d -p 8080:80 hello
docker run --name lawyer-service -p 8080:8080 lawyer-service:0.0.1-SNAPSHOT

// bind multiple port 
## docker run -d -p 8080:80 -p 3000:80 hello

## docker run -p 27017:27017 -d mongo

## docker build -t apigateway . 
## docker build -t apigateway -f dockerfile . 
## docker compose up -d

## docker logs --follow
## docker stop containerid
