# **HOW TO COMPILE AND EXECUTE CPP PROGRAM FILES IN LINUX**

# STEPS
## step 1. Open terminal.
## step 2. Check whether you have g++ complier in your system.
There are Two ways You can check for g++ compiler

``` $ dpkg --list command ```
  
when you run this command you will get list of compiler your system has.in which you can find for g++ compiler.
  
``` $ g++ --version/ gcc --version ```
  
when you run this command you will get like this message on terminal.

![image](https://user-images.githubusercontent.com/63588827/80830434-907c9e80-8c06-11ea-895a-0500627bcacc.png)

If you are getting error finding g++ compiler then you can run this command

```$ sudo yum -y install gcc-c++```

using this command you can install g++ compiler.

## step 3: make one folder name 'cpp'.

``` mkdir cpp```

then go that directory/folder by command 

```cd cpp/```

## step 4: create new cpp file in vi editor

``` vi addtwono.cpp```

press 'i' and go in the insert mode.you can check for insert mode at the end of the terminal then write your code in vi editor

![image](https://user-images.githubusercontent.com/63588827/80832469-5b724b00-8c0a-11ea-8b8e-2d9f7dae6ffe.png)

    
  


