
# FROM: = SELECT YOUR BASE OS
  apna os chunno jispe tum kaam karoge
# RUN := Package aur jo configuration karte hai Os k liye
  matlab jo v necessary hai os k liye like adding user,install 

# CMD := It will execute during container creation
  Matlab container create hone k baad jo pehla chiz run kare

# LABEL := iS LIKE FILTERING WHERE WE HAVE KEY AND VALUE

# Copy : It is used to copy the file from local aur copy one file to another

# ADD: Similar to copy But 2 extra thing
Ye unzip kar leta hai aur online se file v download kar lega

# Expose: Through which port you want to access

# Entrypoint: cmd ki tarah h bas isko override nahi karsakte hai best practices hai ki cmd aur entrypoint ko dono ko use kare

# User:= RUN useradd avinash
        USER avinash

        Qki hum nahi chahte hai ki pura resources ek container use kare to give root access to container

# ARG:=   ISSE BUILD TIME VALUE DIYA JAATA HAI(iMAGE cREATION)

# env:= CONTAINER RUN HOGA TAB HI ACCESS HO PAYEGA (IMAGE RUNTIME)

# ONBUILD: TEMPLATE HAI JISSE KOI AUR USE KAR PAYEGA 

cOMMAND:=

suppose tmhare paas image nahi hai toh you can pull images from dockerhub

# dockerhub: is a place where all the images available

Docker pull nginx

it will the nginx and i didnt give the version so it will pull the latest image 

Docker image nginx:perl

To see all the images:= docker images

To create conatiner which will be create from images: docker create image_id

To run container: docker run container_id 

so in background this command will goes to cmd so if there is no cmd this will terminates quickly

To stop container:= docker stop container_id

How to create ,start and pull images in one command:= docker run nginx

If i want to see the images in local host

docker run -d -p 80:80 image_id

to remove all images based on id:= docker rmi `docker images -a -q`

to remove all container:= docker rmi `docker ps -a -q`

to remove particular images:= docker rmi image_id

to remove particular conatiner := docker rmi container_id

AGAR  LABEL se image sko filter karna hai toh

docker images --filter label=COURSE=DEVOPS


