# Objective-Smalltalk Container
Dockerfile and binaries to create a docker container for running stsh, the Objective-Smalltalk shell.

To create the image, run 

```
./build 
```
For me this creates a 187MB image.   Which is still less than ideal, but better than the 1.2GB development image.

To run the image:

```
docker run --name stsh-deploy -t -i stsh-deploy 
```

To run stsh:

```
./stsh
```

Some very basic things to try:

```
3+4
stdout println:"Hello World!".
a := 3+4.
stdout println:"Hello result: {a}!".
https://wwww.amazon.com/
https://www.amazon.de length
file:.
file:README.md
file:README.md length.
1 to: 10.
(1 to: 100) reduce + 0.
1 to: 100 | sum.
stdout do println: (1 to:10) each.
!ls | wc
class NSArray { -power { self reduce * 1. } } 
#(2,3,4,5) power

```

