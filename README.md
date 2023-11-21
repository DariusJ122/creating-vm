![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/db2a3499-14ac-47d6-a064-e72a82424984)


<h1>Creating a VM in Azure!</h1>
This tutorial outlines the process of creating a VM using Microsoft Azure.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Link to the Azure Portal: https://portal.azure.com

<h2>First Steps</h2>


1.) The first thing you are going to want to do is create a virtual machine by going to https://portal.azure.com/. First login to azure. You should see the home screen, that looks like this image below.

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/d8654579-f33b-43ea-a647-17e678b41717)


2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/152bc1a5-7b5b-4477-b52e-a8bcb896dbc6)

</p>
<br />

3.) You should now see the homepage of the Virtual Machine tab.


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/ec7847d6-df05-4c80-b958-c7b529e9e175)


4.) Click on the top left dropdown where it says Create, and choose Azure Virtual Machine.

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/a543e6f5-3494-4a74-9949-868bf4f3567d)



5.) Now you're in the process of choosing your Virtual Machine specs.

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/25da5004-c440-42ea-8a6f-c5af7c0bc823)



6.) Start off by making sure you have a current subscription, and we're going to name this Virtual Machine "VM-1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For the experiment I'll select Sweden Central. Than we're going to choose Windows 10 for the image.


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/3c84fdaa-6d34-4c21-994c-1a971fd8e288)

  
7.) Now choose the size, we'll use "2 VCPUS,16 GIB Memory", and our username will be "labuser1" and the password will be "Password1VM1" make sure you click the windows checkbox, and than hit review and create!
  

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/d814bb6a-2fcd-4033-af56-ee8bf35f0705)


8.) You should get a validation passed, and than hit create.


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/c5ece425-49a0-4965-816c-85c2c9a8b295)


9.) Allow the Virtual Machine to deploy, ths may take a few minutes,
  
 
 ![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/b785bc26-a8f4-4469-a8f1-8c002b960368)

 
10.) The deployment should now be complete.


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/d4fe96dd-57c4-4b7c-8ca3-bc731da6e984)


  
11.) Click go to resource, it'll take you straight to the VM.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/a3dd341d-2b42-4689-aa2d-604de262af70)



12.) You may see a lot of things going on, but for now just focus on the public IP address, that's what we want. So copy that.
  


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/2f214fa9-6294-4c7c-bdde-f8a7a110baad)



13.) Now press the windows key either on your keyboard or on the screen. Type "RDC" and you should see "Remote Desktop Connection" click that.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/b4f8c813-5d0f-422a-b6f8-15e013ef20bd)



14.) You should see the login pop-up, now paste that IP address into the pop-up, and hit connect.
  


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/541506b0-d22d-4573-b677-19944add757c)




15.) You'll now be prompted to log in with a username and password. Using the one we created in the beginning log in, (labuser1 - username, Password1VM1 - passsword) you should see a prompt saying "Do you want to connect anyways?" Click yes.
  

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/47c8d178-d487-4c83-bd42-8d1f4892e305)




16.) You should be taken inside the Virtual Machine, if you used the labuser1 name, it should log you in to the Virtual Machine as "labuser1", you'll than see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.

  

![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/c578c38b-0ea9-4749-95d8-72f28b46cd88)



17.) You're now inside a virtual machine! Now remember I selected Sweden as my Virtual Machine location. What do you think my Google would look like? Boom! Because I set my Virtual Machine location to Sweden it acts as a computer connected to a network in Sweden! Pretty cool right?



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/73736361-d0c0-40b7-9dd8-5c8c11cfc244)




18.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"



19.) Now you should be back inside the Azure Portal, and looking inside the Virtual Machine specs and settings. Now click delete.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/dd2ea6d0-c3bd-481a-a17c-1400ec15859f)






20.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/9f82323b-8061-40b1-bfb5-9c1a8c91de0c)





21.) Boom. Should be done now. Going back to the Home for the Virtual Machines, it should be cleared out.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/d494812a-f287-44a5-9701-a9fd9422af0e)






22.) Now you're not quite done yet. Click the search bar and type "Resource Groups", you should now be looking at your current resource groups.



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/db4e58b1-669e-4a26-8d7a-01c27aaa8cbf)




23.) Now click that Resource Group whcih was automatically created when we created our Virtual Machine. And now click "Delete Resource Group". 



![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/9c96c82b-90ff-4771-afdf-63472ee13bc4)




24.) Now type the name of the resource group, and click delete.


![image](https://github.com/DariusJ122/osticket-prereqs/assets/150752364/913a508f-e2e0-4175-a5b4-91135073be4b)


25.) CONGRATS!! You have now created your first Virtual Machine! Here's also a link to a creator who I watch pretty often, who's discussing some creative ways you can use a Virtual Machine - https://technotim.live/posts/20-ways-virtual-machine/
