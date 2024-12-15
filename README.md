<p align="center">
<img src="https://github.com/user-attachments/assets/0bd56848-80ce-43c0-92b5-dd0aba7701c9"/>

</p>

<h1>Configuring a VM and Finding its IP in (Azure)</h1>
This tutorial outlines the implementation of creating a Windows VM using Azure configuring it and remote desktop connecting to that VM, and then using Powershell to identify the IP Adress..<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- PowerShell

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1 : Create a Resource group for the VM
- Step 2 : Create the VM 
- Step 3 : Remote Desktop to the VM
- Step 4 : Use Powershell to find the IP adress within the VM 

<h2>Deployment and Configuration Steps</h2>

<p>

<img src="https://github.com/user-attachments/assets/2761320d-4a46-44dd-b667-ecb3a7c8c81c"/>
<img src="https://github.com/user-attachments/assets/58ba659e-0fff-4b2f-a6fa-36edf9d5fc1b"/>
<img src="https://github.com/user-attachments/assets/5ddd6670-0cae-4a76-9c0c-57606e0a6dab"/>
<img src="https://github.com/user-attachments/assets/c36de276-8760-4b54-be30-52786d59493d"/>
<img src="https://github.com/user-attachments/assets/31f6473e-f51b-4acc-bd6f-6682ed0c1825"/>







</p>
<p>
Here in this demostration we are creating the resource group and the Vm, we want to make sure we create the names and passwords to something we remember as that is what we will use to login to remote desktop. We want to select the Windows 10 os and combined that with the 2 cpu size and make sure that lisence box is checked at the very bottom. Lastly make sure that the Vnet is created to the one you pick and review and create.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0afe92ef-0491-4ab7-9052-b690c1830c15"/>
<img src="https://github.com/user-attachments/assets/a9c18085-87e7-41c2-bc8a-f97f795d27ff"/>
<img src="https://github.com/user-attachments/assets/bc22f968-1615-4863-a99b-dcce8f7f601c"/>
<img src="https://github.com/user-attachments/assets/39ac39d3-0653-4872-a1ee-86541eda2b6e"/>
<img src="https://github.com/user-attachments/assets/3be4d41e-b2a5-4de5-97c0-46ca316b1e7e"/>



</p>
<p>
In the next step we are remote connecting to the windows 10 vm in which we want to make sure its up and running first where it shows its IP where we can either copy it from right there in the VM tab or click on the vm itself and copy it from there. Next we open up Remote Desktop Connection if we are on windows and paste the IP adress of the Vm and we get the login screen where we use the login info. Make sure the information is correct so write it down on a notepad and finally let it run through and sign in.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/86b4d6ec-0252-407a-a1db-1f7cf2280161"/>
<img src="https://github.com/user-attachments/assets/5e616b48-687f-49a3-8735-14ca2117b750"/>


</p>
<p>
For the final step we want to get all logged in and open up PowerShell as shown. Once that is done we want to type in the command "ipconfig" where it gives the IPV4/IPV6 adress where the IPV4 may not looked like the one we copied because this one is the private version as shown in Azure. This is how you create a VM using azure and finding the Private IP of such VM without looking through azure.
</p>
<br />
