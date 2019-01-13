# objective-smalltalk-container
Dockerfile and binaries to create a docker container for running stsh, the Objective-Smalltalk shell

To create the image, run ./build 

For me this creates a 187MB image.   Which is still less than ideal, but better than the 1.2GB development image.

To run the image:

docker run --name stsh-deploy -t -i stsh-deploy    /bin/bash -l


To run stsh:

su -l gnustep

./stsh


