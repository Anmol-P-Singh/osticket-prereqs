<p align="center">
<img width="403" height="65" alt="image" src="https://github.com/user-attachments/assets/95416299-a06d-42a8-a81f-ad82de7cd432" />



</p>

# Accessing Windows 10 Remote Desktop on Azure VM via Public IP

This tutorial will walk you through setting up and connecting to a Remote Desktop (RDP) session on an Azure Virtual Machine using its public IP address.

## Prerequisites Needed for the Tutorial

- Microsoft Azure account
- Basic knowledge of Azure Virtual Machines
- RDP client (e.g., Windows Remote Desktop, Microsoft Remote Desktop for macOS)

## Operating Systems Used

- Microsoft Windows 11 (21H2)

## Installation Steps

1. Go to **Resource Groups** in Azure by using the search bar.
2. Click on **+ Create**.
   
   ![Create Resource Group](https://github.com/user-attachments/assets/aac66d07-7c50-43fa-882d-53fd0e805968)

3. Create a resource group name.
4. Pick a region of your choice and don't forget it—because it will be used again when creating the Virtual Machine.
5. Click **Review and Create**.
6. Click **Create** when ready.

   ![Resource Group Creation](https://github.com/user-attachments/assets/fc25e85e-ebaf-4e1d-bd08-47c19af5b155)

<img width="605" height="197" alt="image" src="https://github.com/user-attachments/assets/f54684c3-79b2-4c8d-9d6d-66dabe628d27" />

- After resource Group is created then go to virtual machines by tying it in the search bar
- click on + create then virtual machine
 
  
<img width="761" height="102" alt="image" src="https://github.com/user-attachments/assets/0ce8f331-8400-4b75-be9c-54a386ab7d50" />

- For resourse groups pick the name of the one that you have created


  <img width="806" height="405" alt="image" src="https://github.com/user-attachments/assets/41187d82-4c1c-4010-83f1-e928b2c2da68" />

- for the VM name it can be the same as the resouce group, but it's better to pick something different so that it's easily identifiable
- Pick the same region for the VM and resource group to reduce data transfer costs, boost performance, and simplify management
- For image pick windows 10 pro and leave 
