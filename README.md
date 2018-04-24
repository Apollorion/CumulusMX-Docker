# CumulusMX - Docker
**For the CumulusMX community**

## Available on Docker Hub
https://hub.docker.com/r/jiinxt/cumulusmx-docker/

    docker run -dit -p 8998:8998 -p 8002:8002 --name cumulus --privileged -v /dev/bus/usb:/dev/bus/usb jiinxt/cumulusmx-docker:latest

## How to build:
  1. Install Docker
  2. Run command

    docker build -t jiinxt/cumulusmx-docker:latest --build-arg TZ=your/tz/data ./Dockerfile
    
## How to run:
  1. Run command:
 
    docker run -dit -p 8998:8998 -p 8002:8002 --name cumulus --privileged -v /dev/bus/usb:/dev/bus/usb jiinxt/cumulusmx-docker:latest
  1. Browse `127.0.0.1:8998`, and setup cumulus
  2. Restart the container:

    docker stop cumulus && docker start cumulus
    
    
I am NOT the author of CumulusMX, I just created an easy container to deploy CumulusMX with. Please see http://sandaysoft.com/ for the creator of CumulusMX.