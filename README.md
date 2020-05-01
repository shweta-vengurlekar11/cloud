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

## step 3: Make one folder name 'cpp'.

``` mkdir cpp```

then go that directory/folder by command 

```cd cpp/```

## step 4: Create new cpp file with help of vi editor

``` vi addtwono.cpp```

press 'i' and go in the insert mode.you can check for insert mode at the end of the terminal then write your code in vi editor

![image](https://user-images.githubusercontent.com/63588827/80832469-5b724b00-8c0a-11ea-8b8e-2d9f7dae6ffe.png)

after complete the code press 'esc' key.after that press ':wq' to write and commmit the changes made to the file.

## step 5: Compile the program

you can compile file by the command below:

```g++ first.cpp```

by this command compiler will create one output file to your directory
but you can name that file by the command below instead of the command above

```g++ first.cpp -o first```

so output file will be created with the name of 'first'.and if file have any compile time error or warnings it will show after running of command.


## step 6: Execute you output file

now command is 

```./first```

this command will give you output.

![image](https://user-images.githubusercontent.com/63588827/80836888-5239ac00-8c13-11ea-90f0-0f69419f7b43.png)

So, these are the steps to compile and execute the cpp files in linux.

here are some more examples to try on:

1. [FUNCTION CALL FROM ANOTHER CLASS](https://github.com/shweta-vengurlekar11/cloud/blob/master/callingfunction.md)
2. [sTRING CONCANATION](https://github.com/shweta-vengurlekar11/cloud/blob/master/concationstring.md)
3. [VIRTUAL FUNCTION](https://github.com/shweta-vengurlekar11/cloud/blob/master/virtualfunction.md)
4. [FIBONACCI SERIES](https://github.com/shweta-vengurlekar11/cloud/blob/master/fibonacciseries.md)

