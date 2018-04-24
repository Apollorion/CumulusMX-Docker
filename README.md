# CumulusMX - Docker
**For the CumulusMX community**

## How to build:
  1. Install Docker
  2. Run command

    docker build -t cumulus:latest --build-arg TZ=your/tz/data /path/to/this/file
    
## How to run:
  1. Run command:
 
    docker run -dit -p 8998:8998 -p 8002:8002 --name cumulus --privileged -v /dev/bus/usb:/dev/bus/usb cumulus:latest
  1. Browse `127.0.0.1:8998`, and setup cumulus
  2. Restart the container:

    docker stop cumulus && docker start cumulus