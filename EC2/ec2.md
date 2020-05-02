# **EC2 (Elastic Compute Cloud)**
- It 8is a IAAS, i.e it provides infrastructure (raw computing resources) as a service.
- Basically you create laptop vairtually, it will be present at your respective datacentre. It also has all resources that are present in your laptop such as processor, RAM, OS, volume(SSD) which we can select according to our need and can be modified easily.
- Its instance is created and becomes available to you in a fraction of seconds and You can remotely login into your EC2 which located in datacenters through SSH so when we created laptop machine on aws with linux os we used mobaxterm software for SSH.

## Steps to create EC2
1. step 1: Go to AWS CONSOLE.Then go to services in the menu bar.
2. step 2: select EC2 from compute section or you can search for 'ec2' in search bar.
3. step 3: Click on 'launch instance'.
4. step 4: Select which AMI You want from the list or ypu can search for AMI from search bar.


![image](https://user-images.githubusercontent.com/63588827/80887577-c50e5a00-8cdb-11ea-8e63-811768e32ed0.png)



5. step 5: select instance type.you can choose family of instance type according to your CPU and Memory requirements.


![image](https://user-images.githubusercontent.com/63588827/80888385-fedf6080-8cdb-11ea-8baa-52293b139f88.png)


6. step 6: Click on 'next:configure details' if you want any changes in the default configurations.


![image](https://user-images.githubusercontent.com/63588827/80890720-c4c28e80-8cdc-11ea-97ab-c63173485187.png)


7. step 7: After configuration setting now you can change storage details according to your requirements.


![image](https://user-images.githubusercontent.com/63588827/80890782-2b47ac80-8cdd-11ea-89ef-400f7a9a1b6f.png)


here you can see i have changed the size of the storage to 30 as per my requirements.
now you click on 'next:add tags'.

8. step 8: Here You can add tag to to your instances.so click on 'Add tag'.write name in key box and value can be any name as per your choice.


![image](https://user-images.githubusercontent.com/63588827/80890896-0273e700-8cde-11ea-9533-2ffb9433d5e2.png)


now click on 'Next:configure security groups.But before that let's understand what is security group.

## Security Group
- A security groups acts as a virtual firewall similar like windows firewall that controls the traffic for one or more instances.
- When we launch (create) an instance, we can specify one or more security groups or we can use the default security group provided by aws.
- security group has inbound and outboud rules which controls incoming and outgoing traffic by enabling/disabling ports respectively.


9. step 9: so now you can create new security group and enter the security group name and description or you can select exsting security groups.


![image](https://user-images.githubusercontent.com/63588827/80890982-be351680-8cde-11ea-9ad4-2f949beff43e.png)


now click on you can click on 'review and launch'.

![image](https://user-images.githubusercontent.com/63588827/80891026-081dfc80-8cdf-11ea-962d-d1de25757cd9.png)


here you will see all your ec2 instance configurations you have choosen.If you want to change some conguration you can click on previous till you go to the page where you want to make any changes.

10. step 10: now you can click on launch.now you will get window for selecting or creating key pair.before that let's understand what is key pair,

A key pair consists of a public key that AWS stores, and a private key file that you store. Together, they allow you to connect to your instance securely. For Windows AMIs, the private key file is required to obtain the password used to log into your instance. For Linux AMIs, the private key file allows you to securely SSH into your instance.

you can select existing key pair or create new key pair.here we are creating new key pair.so select 'create new key pair' from dropdown and give name to the key pair.


![image](https://user-images.githubusercontent.com/63588827/80891251-6f887c00-8ce0-11ea-8189-8cf0ad56f166.png)


11. step 11: Click on download key pair.it is important to download the key pair pem file.it will need to create ssh for you instance.

12. step 12: now click on launch instance.


![image](https://user-images.githubusercontent.com/63588827/80891323-e3c31f80-8ce0-11ea-9f48-0d2f19427085.png)


done...you can see you instance which can be like your laptop which is created in hardly 10 minutes.


here you can see your instance creation status.

now you can click on view instance list.and now yon are able to see the instance list.


![image](https://user-images.githubusercontent.com/63588827/80891391-4c120100-8ce1-11ea-8332-d04e31facaa3.png)


13. step 13: now you can change your instance state by selecting instance then click on 'Actions' in the menu,now select 'stance state'
from the options.


![image](https://user-images.githubusercontent.com/63588827/80891501-043fa980-8ce2-11ea-9312-8ff246b7cd32.png)


instance states:

- start: if your instance is in the stopped state you can again state by selecting start state.
- stop: if you dont have use of your current instance you can stop it so it will affect on your cost which you are paying for your instance.for stopped instance you are only paying for your storage spcae and not for CPY and MEMORYY.
- Terminate:you can permanently delete your instance by changing to this state.






