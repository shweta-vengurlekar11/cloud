# **SNS (Simple Notification service)**

- it can notify you with email or sms for an event happening on aws cloud
 eg:if you upload any file to your buckect so through SNS u will get email to notify the uploading ofthe file.
- Mainly it contains topic and subscription.
- U can create multiple topics for different events.

## what is subscriber and publisher?
- in simple word we can say publisher(aws) is sender and subscriber is receiver(we).
 
## Steps to create topic:

1. step 1: Go to AWS CONSOLE.Then go to services in the menu bar.
2. step 2: you can search for 'SNS' in search bar.
3. step 3: Now enter a topic name and Click on 'Create Topic'.

![image](https://user-images.githubusercontent.com/63588827/81055459-53eec280-8ee6-11ea-9c0f-e4c17ae6c822.png)


4. step 4: enter display name.

![image](https://user-images.githubusercontent.com/63588827/81056079-8a790d00-8ee7-11ea-8194-24e52cfc608c.png)


5. step 5: Make changes to the access policy as shown below.


![image](https://user-images.githubusercontent.com/63588827/81056318-fa879300-8ee7-11ea-9b1a-f7d5f419001a.png)


6. step 6: In IAM role present in Delivery status logging click on create new service role.we need to enter ARN for IAM's.Now we are going to create IAM roles here.

![image](https://user-images.githubusercontent.com/63588827/81057222-a087cd00-8ee9-11ea-926d-13d1036b344f.png)


so right click on create role.it will open new window.on that window u will file creation for two roles do not change anything and click on Allow.


![image](https://user-images.githubusercontent.com/63588827/81057400-f3fa1b00-8ee9-11ea-91c3-3474b73ba0f9.png)


now we have to use this role in our topic.so again go to the topic creation window.and select use existing service role.here  we are not getting the list for IAM's so we have to go to IAM services window.for that go to services menu.search for IAM.go to IAM window.click on roles in left side menu.


![image](https://user-images.githubusercontent.com/63588827/81056903-0aec3d80-8ee9-11ea-8ecc-49df1df420b1.png)


7. step 7: search for SNS in the search.you will get two roles which you have just created.


![image](https://user-images.githubusercontent.com/63588827/81057738-a29e5b80-8eea-11ea-952c-3ff81f33aab4.png)


select SNSFailureFeedback.go inside.copy its ARN.


![image](https://user-images.githubusercontent.com/63588827/81057875-e729f700-8eea-11ea-8dbc-d88885e1a33b.png)


and paste it to the IAM role for successful deliveries box.and do it same for IAM role for failuer deliveries


![image](https://user-images.githubusercontent.com/63588827/81058216-96ff6480-8eeb-11ea-93c6-1cd959eb4b1a.png)


Now click on 'create topic'.then you will see your topic in the list.


![image](https://user-images.githubusercontent.com/63588827/81058323-d4fc8880-8eeb-11ea-870d-2a85ab79f996.png)


8. step 8: click on create Subscrption as you see in above image.

select Email from the list of protocol.Enter your email-id.and click on create subscription.


![image](https://user-images.githubusercontent.com/63588827/81058499-30c71180-8eec-11ea-9ca0-3b9038c96f5f.png)


9. step 9: you will see status for Subscrption is still pending.


![image](https://user-images.githubusercontent.com/63588827/81058672-87cce680-8eec-11ea-9a38-4dd568fb46e2.png)


10. step10: for that you have to confirm the subscrprition from the link which is sent to you in your email.


![image](https://user-images.githubusercontent.com/63588827/81058889-0033a780-8eed-11ea-8b31-8afbb5da2142.png)


after confirming you wil see like image below.


![image](https://user-images.githubusercontent.com/63588827/81058973-2bb69200-8eed-11ea-81b5-9a24febb1cdc.png)


now you canse status is now confirmed.


![image](https://user-images.githubusercontent.com/63588827/81059052-51dc3200-8eed-11ea-81c6-0217872bb8b4.png)


you can now see our SNS topic is ready.remember you have to create subscription for each topic you are creating.


## let's use SNS to our S3 event.(s3 as publisher)


1. step 1: Go inside your already created s3.Go the properties and select Events.click on add notification.


name the event.select All object create events from the options.then select 'SNS' in sent to options and select your created SNS topics from the options.


![image](https://user-images.githubusercontent.com/63588827/81060068-599cd600-8eef-11ea-898f-6fdccbf74d64.png)


now you have 1 active event on s3.

2. steo 2: go tooverview in menu.upload 1 file after successfull uploading check if get a email or not.


yes we get email will the details.


![image](https://user-images.githubusercontent.com/63588827/81061064-4e4aaa00-8ef1-11ea-9d24-b8bd09b410e0.png)



## let's use SNS to our Ec2 alarm.(EC2 as publisher)

1. step 1: select 1 ec2 from the list.click on create status check alarm.


![image](https://user-images.githubusercontent.com/63588827/81062014-ebf2a900-8ef2-11ea-9858-8586b0bfc338.png)


select sent to and select your sns from options.choose your alarm configurations as below image


![image](https://user-images.githubusercontent.com/63588827/81061898-c8c7f980-8ef2-11ea-8741-007de994e6aa.png)


stop and start gain your EC2 for alarm status change.Now you will get email as per your alarm configurations.
