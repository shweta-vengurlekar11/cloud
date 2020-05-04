# **Lambda (function)**

- it is serverless cloud computing service provided by aws.
- if you store any file in ec2 you have to pay for storage but in lambda you can store many codes but for storage it will not cost you anything.It will charge you only at the time of execution of code.
- for the period a program or code you are running,aws will charge you for CPU and RAM usage.
- and also there will be no charge for os you are using because the service is severless.
- Scalibility: Automatic changes of resources according to need for running a code (scale up and scale down).
- paralization: this function can be used according to request at the same point of time.many people can use this function at the same time.


## steps for creating lambda function

1. step 1: Go to AWS CONSOLE.Then go to services in the menu bar.
2. step 2: select Lambda from compute section or you can search for 'Lambda' in search bar.
3. step 3: Click on 'create function'.

![image](https://user-images.githubusercontent.com/63588827/80922033-ee8cbb80-8d97-11ea-89e0-3ef23244db4a.png)


4. step 4: select 'use blueprint' for existing function provided by aws.after that you can search with keyword whiever function you want.here we are searching for
hello world program.we will get available option for function we aresearching for.


![image](https://user-images.githubusercontent.com/63588827/80922162-c5b8f600-8d98-11ea-881b-24b5f9c24857.png)


5. step 5: click on 'configure'.
6. step 6: now you can name your function.then select 'use existing role' and select role from the dropdown.


![image](https://user-images.githubusercontent.com/63588827/80922184-ed0fc300-8d98-11ea-9899-8b7178510b0f.png)


7. step 7: scroll down.and you can see the code in the laguage you have selected.now to create function you can click on 'create function.


![image](https://user-images.githubusercontent.com/63588827/80922254-71fadc80-8d99-11ea-96aa-536dfb02a8d7.png)


here we can see our function is created.

![image](https://user-images.githubusercontent.com/63588827/80922279-a373a800-8d99-11ea-9255-d6af88c759b7.png)


Alternatively you can choose 'author from scratch' while creating a funtcion.
you need to proivde the code and then run.Click on author from scratch then enter the function name.


![image](https://user-images.githubusercontent.com/63588827/80922358-33b1ed00-8d9a-11ea-9ce8-92d9a4e8899e.png)


you can then select the language of your choice.Then click on create function.

![image](https://user-images.githubusercontent.com/63588827/80922398-71af1100-8d9a-11ea-9a67-1b4273978d4f.png)

but now we are using blueprint function.so lets continue with that.


8. step 8:click on the function in the list.then Scroll down you will see the code,now you can make changes in the code if you want.
If you made any changes click on save and then on test.


![image](https://user-images.githubusercontent.com/63588827/80922472-f69a2a80-8d9a-11ea-9bac-f03868131530.png)


9. step 9: Enter the event name and you can change the key values e.g i have entered hey in place of value1 and event in the place of value2,bye in the place of valuue 3 and also i have changed the key3 name as test.
and now you can click on create.


![image](https://user-images.githubusercontent.com/63588827/80954301-c2fee500-8e1a-11ea-9216-2eefdc9ef12f.png)



10. step 10: You can see on the window i have change key3 value to test,if you will not change this to test then it will give you undefined value at key3.and also dont forget to save the changes you have made.then click on test.


![image](https://user-images.githubusercontent.com/63588827/80957851-9ef2d200-8e21-11ea-9f9d-ff06905b5d6d.png)


11. step 11: scroll up and click on details.you will see all the details for execution of code.


![image](https://user-images.githubusercontent.com/63588827/80958401-9c44ac80-8e22-11ea-977d-ac192144dd01.png)



you  can see output and your changed values in the output.


![image](https://user-images.githubusercontent.com/63588827/80958534-d01fd200-8e22-11ea-8c3b-cf0bd0b7a659.png)


12. step 12:whenever you do not need a function you can delete the function by selecting it from the list.


![image](https://user-images.githubusercontent.com/63588827/80922682-55ac6f00-8d9c-11ea-938e-4190518c49ce.png)



## NOW WE WILL SEE LAMBDA AS A EVENT DRIVEN (AUTOMATED) SERVICE

we are going to fire lambda function whenever any file uploaded to s3.for that we have to follow steps given below:

1. step 1: Go to the S3 services.
2. step 2: go to Any bucket you want or create bucket and click on the bucket name.
3. step 3: now go to properties menu.there you will find 'event' in the advanced settings.click on the events.
4. step 4: click on 'add notification'

![image](https://user-images.githubusercontent.com/63588827/80960431-75887500-8e26-11ea-9d71-355bb83e27e3.png)


5. step 5: give name to the event.select the events details.prefix and suffix are used for event trigger.eg if you want to trigger lambda function only if any file name with cdac suffix of cdac prefix is present.then you can select 'sent to' from the dropdown to which you want send the event trigger and  then selection lambda function present in the dropdown.and then click on 'save'.


![image](https://user-images.githubusercontent.com/63588827/80960601-cf893a80-8e26-11ea-98b1-18e44b4c4642.png)


6. step 6: now select the event and click save.


![image](https://user-images.githubusercontent.com/63588827/80960967-91404b00-8e27-11ea-90a4-a1e052b404c5.png)


7. step 7: now open lambda to the new window.
8. step 8: go to your lambda and do some changes then you can find out some difference in execution so that you can differentiate between old and new lambda function.after changes click on save do not test it.

![image](https://user-images.githubusercontent.com/63588827/80961319-55f24c00-8e28-11ea-9896-de16dd0c1e68.png)


9. step 9: again go to your s3 and upload any one file to the s3.


![image](https://user-images.githubusercontent.com/63588827/80961471-a9649a00-8e28-11ea-89ab-c797575be175.png)


10. step 10: after successfully uploading the file.you can search for 'cloudwatch' in services.open cloudwatch in the new window.
there you can see even fired in the list.


![image](https://user-images.githubusercontent.com/63588827/80962522-d154fd00-8e2a-11ea-8890-b9e7041ddf76.png)

