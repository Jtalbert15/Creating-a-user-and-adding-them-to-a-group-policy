# Creating-a-user-and-adding-them-to-a-group-policy
In this Lab I will create a user to our Domain and add them to a group policy.

Prereqs
1) https://github.com/Jtalbert15/Installing-Virtual-Machine-and-Windows-ISO-s
2) https://github.com/Jtalbert15/Setting-up-Active-Directory-on-our-Windows-Server-2019
3) https://github.com/Jtalbert15/Adding-A-computer-to-our-domain

Now we can get started

Step 1) Open up your Windows Server 2019 Machine and log in

<img width="622" alt="Screenshot 2024-05-20 at 9 45 24 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/9286a5b9-d949-48d9-b87c-8c3bfd9adb5c">

Once you see this screen click on the Tools button in the top right corner of your screen

<img width="622" alt="Screenshot 2024-05-20 at 9 46 50 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/6f1314bb-d232-4e80-a5b4-faaf2e03a61b">

Select Active Directory Users and Computers

<img width="620" alt="Screenshot 2024-05-20 at 9 47 49 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/14c2636c-9a36-4592-a1d5-13d0098ae37b">

Select your domain you created. Yours may be different if you chose a different domain name.

<img width="621" alt="Screenshot 2024-05-20 at 9 49 23 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/a786f58a-e53d-43c9-9d10-6aef56b84861">

Now we are going to double click on the Users file


<img width="620" alt="Screenshot 2024-05-20 at 9 50 04 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/034d67b9-7b4f-45ff-8286-e4e9d3af5b10">

<img width="620" alt="Screenshot 2024-05-20 at 9 50 45 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/4f8ec685-29ee-4da3-a1f1-0d0b73be105b">

At the top of the window you should see a task bar select the singular user with the orange star next to him

<img width="636" alt="Screenshot 2024-05-20 at 9 55 49 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/2003e942-8fbb-4320-bb0d-2b60fe7e199a">

Now we can create our user. You may fill in these fields to your liking. Make sure you remember the logon name you give the user as this will be the username that we log into when we are using this users account

<img width="634" alt="Screenshot 2024-05-20 at 9 58 27 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/26b1fc28-4f4c-4e86-a79b-474b1cb6c8d5">


<img width="267" alt="Screenshot 2024-05-20 at 9 53 33 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/aa64182d-024a-457a-aa1c-5f4c17e7fc00">

Once you have filled out the information to your liking click next

<img width="634" alt="Screenshot 2024-05-20 at 9 59 34 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/514f3f40-c445-401a-bbc4-9e3b95684cbf">

Now we are going to make a password for this account. Usually we would leave the User must change password on logon checked so we don't know the users password. Since we want to know their password we will uncheck

<img width="636" alt="Screenshot 2024-05-20 at 10 03 13 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/b6db0ba9-075a-4b7b-8be8-ad0a8403ca19">

Once done click next

<img width="637" alt="Screenshot 2024-05-20 at 10 05 57 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/e3d121a3-cf01-4d17-a79e-77749389c42b">

Finally click Finish

<img width="467" alt="Screenshot 2024-05-20 at 10 06 50 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/e2d7ee78-caca-4c7f-9338-03377b039274">

And there we are. Congratulations you added a user to the domain!

Before we log into our account lets add our user to a group policy

Step 2) Adding a user to a group policy

<img width="635" alt="Screenshot 2024-05-20 at 10 08 58 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/1e006bb5-1a56-4eb0-8271-95873f2c46c9">

To start we are going to double click on the user

<img width="633" alt="Screenshot 2024-05-20 at 10 09 40 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/907895a5-2455-4ef5-83c3-ff0dfa4a2f13">

Then we are going to click on Member Of in the top left corner of the window

<img width="638" alt="Screenshot 2024-05-20 at 10 10 53 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/7efa62f2-4ffa-4a0d-bbfe-9ff4201029f2">

You can see we are already a member of the Domain users group 

Lets give ourselves admin powers. Click Add...

<img width="638" alt="Screenshot 2024-05-20 at 10 12 35 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/9d7d1286-9a29-4147-9e15-ae9774e077ec">

Where our cursor is you can type admin

<img width="282" alt="Screenshot 2024-05-20 at 10 13 37 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/f47bc57a-f554-4f4c-85b6-8dbbaaebcf54">

To the right there is a button that says Check Names. Click it

<img width="286" alt="Screenshot 2024-05-20 at 10 14 38 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/c3f814e1-a6ae-4823-949d-9682ea6c2be0">

Our computer searched and found the Administrators group. This is the group we want so you can click OK

<img width="636" alt="Screenshot 2024-05-20 at 10 15 39 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/233f0103-9c0b-4711-b4d5-aa5990eb3d44">

In order for this to take effect we are going to click apply at the bottom of the window followed by OK

Now after double clicking the user and selecting Member Of you should see that our user is now a part of 2 groups.

Now we can sign into our Windows 10 VM with our login credentials we gave our user!

Step 3) with your Server VM still running boot up the windows 10 VM

<img width="634" alt="Screenshot 2024-05-20 at 10 22 21 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/dc580268-8328-40c5-afa1-5a862f0f4ac0">

We do not want to log on as the local admin to the computer so click other user in the bottom left corner 

<img width="631" alt="Screenshot 2024-05-20 at 10 23 21 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/00f9fbb7-6c67-4c76-9851-ac1328a39e15">

Now we can log in with the credentials we gave our new user

<img width="635" alt="Screenshot 2024-05-20 at 10 24 49 AM" src="https://github.com/Jtalbert15/Creating-a-user-and-adding-them-to-a-group-policy/assets/66844406/b26123f2-d01e-4265-b82b-c5efa8bae675">

Congrats! You have logged into the domain as the user we just created!

