# objective-smalltalk-container
Dockerfile and binaries to create a docker container for running stsh, the Objective-Smalltalk shell

To create the image, run ./build 

To run the image:

docker run --name stsh-deploy -t -i stsh-deploy    /bin/bash -l


To run stsh:

su -l gnustep
./stsh


