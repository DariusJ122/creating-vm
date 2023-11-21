![image](https://github.com/DariusJ122/creating-vm/assets/150752364/a31856fc-efdf-4c2d-b665-2ed272e62cd1)



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

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/5800872a-0bf5-44df-a136-8f30fa175ddb)


2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/9aba926a-4b3e-4ed7-b554-00a5667fe928)

</p>
<br />

3.) You should now see the homepage of the Virtual Machine tab.


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/724bd162-cb12-4185-b573-35f1df069680)


4.) Click on the top left dropdown where it says Create, and choose Azure Virtual Machine.

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/f44ee44e-c442-4121-b425-092189b15a01)



5.) Now you're in the process of choosing your Virtual Machine specs.

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/33d99957-1902-462f-9968-13be05a61342)



6.) Start off by making sure you have a current subscription, and we're going to name this Virtual Machine "VM-1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For the experiment I'll select Sweden Central. Than we're going to choose Windows 10 for the image.


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/81a158ab-e996-408a-b098-76f61dbb337d)

  
7.) Now choose the size, we'll use "2 VCPUS,16 GIB Memory", and our username will be "labuser1" and the password will be "Password1VM1" make sure you click the windows checkbox, and than hit review and create!
  

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/ac731d30-bbff-4441-8286-047c6a5ccc8f)


8.) You should get a validation passed, and than hit create.


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/a170b46b-8ef9-42b1-bc35-e3de963757f3)


9.) Allow the Virtual Machine to deploy, ths may take a few minutes,
  
 
![image](https://github.com/DariusJ122/creating-vm/assets/150752364/9445276f-196e-4356-92b2-631f23deb15a)

 
10.) The deployment should now be complete.


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/db14674a-db3f-48b6-a947-0448a7fadb81)


  
11.) Click go to resource, it'll take you straight to the VM.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/fcb29827-2cda-46fa-8e00-84c388d6bafb)



12.) You may see a lot of things going on, but for now just focus on the public IP address, that's what we want. So copy that.
  


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/89996581-9e09-4788-8fbd-0514f6d405d5)



13.) Now press the windows key either on your keyboard or on the screen. Type "RDC" and you should see "Remote Desktop Connection" click that.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/45380f85-a41c-4cae-a036-02e888a0fb87)



14.) You should see the login pop-up, now paste that IP address into the pop-up, and hit connect.
  


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/45239334-14ca-4281-8851-feb674500d12)




15.) You'll now be prompted to log in with a username and password. Using the one we created in the beginning log in, (labuser1 - username, Password1VM1 - passsword) you should see a prompt saying "Do you want to connect anyways?" Click yes.
  

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/01524929-4735-459f-b73d-ce15c9448abb)




16.) You should be taken inside the Virtual Machine, if you used the labuser1 name, it should log you in to the Virtual Machine as "labuser1", you'll than see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.

  

![image](https://github.com/DariusJ122/creating-vm/assets/150752364/3a42d681-fe82-4d15-b3a9-99eeba318d94)



17.) You're now inside a virtual machine! Now remember I selected Sweden as my Virtual Machine location. What do you think my Google would look like? Boom! Because I set my Virtual Machine location to Sweden it acts as a computer connected to a network in Sweden! Pretty cool right?



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/03e0dbfb-4f64-4386-aa1c-7331af3037d2)




18.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"



19.) Now you should be back inside the Azure Portal, and looking inside the Virtual Machine specs and settings. Now click delete.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/24d5818d-7919-4358-a61c-a366e896a3da)






20.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/0a7c2e47-4f63-40c9-930d-7a1923b73cab)





21.) Boom. Should be done now. Going back to the Home for the Virtual Machines, it should be cleared out.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/5f883ad2-36b6-4515-8af6-536b057670e8)






22.) Now you're not quite done yet. Click the search bar and type "Resource Groups", you should now be looking at your current resource groups.



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/a9f69598-7895-44de-ba69-76bfa7e6cbb0)




23.) Now click that Resource Group whcih was automatically created when we created our Virtual Machine. And now click "Delete Resource Group". 



![image](https://github.com/DariusJ122/creating-vm/assets/150752364/9be1c1ea-bba5-42bc-8c63-864813aac09b)




24.) Now type the name of the resource group, and click delete.


![image](https://github.com/DariusJ122/creating-vm/assets/150752364/cf42e946-243e-41dc-ab65-f4b183623390)


25.) CONGRATS!! You have now created your first Virtual Machine! Here's also a link to a creator who I watch pretty often, who's discussing some creative ways you can use a Virtual Machine - https://technotim.live/posts/20-ways-virtual-machine/
