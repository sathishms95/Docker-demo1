 TO RUN THE WEBSERVER USING DOCKERFILE . 
 
 Create a Dockerfile in the same directory
 
 $ vi dockerfile
 
 And paste the below commands in Dockerfile
 
 $ FROM nginx
   COPY . /usr/share/nginx/html
   
 To create a Docker image run:
 
 $ docker build -t my_image .
 
 Run your Docker container using the newly created image
 
 $ docker run -it -d -p 8080:80 my_image
 
 Note : (8080:80 as host port: container port)
 To view the image in AWScloud9 click on Preview to view the application or webserver .The cloud9 preview only work on port 8080 . So expose the container to 
 8080.
 
 To run the application from images directly from dockerhub

$ docker push sathishms95/docker_slick_webapp:tagname  
 
 
   
   
 
