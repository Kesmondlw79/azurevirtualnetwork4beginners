# azurevirtualnetwork4beginners

Azure Virtual Network Setup Lab

## Introduction

Welcome to the **Azure Virtual Network Setup Lab**! In this lab, you will learn how to create and configure a secure and scalable virtual network within Microsoft Azure. Virtual networks (VNets) are a foundational component of cloud-based infrastructure, enabling the communication between Azure resources and providing a secure environment for your applications and services.

Azure Virtual Networks are crucial for ensuring secure and isolated communication between resources within the cloud, preventing unauthorized access. They enable seamless connectivity with on-premises infrastructure, allowing for hybrid cloud scenarios and secure data exchange. By providing control over IP addressing and scalability, VNets offer flexibility to grow your infrastructure while optimizing performance and cost-efficiency.

This guide will walk you through the steps required to set up an Azure Virtual Network from scratch, covering key concepts such as subnets, network security groups (NSGs), and routing. By the end of this lab, you will have a fully functional Azure Virtual Network tailored to your specific needs, providing you with a solid understanding of how networking works in the Azure cloud environment.

Lab: Create a Virtual Network (VNet)
Goal:

•	Understand the concept of cloud deployment models (Public, Private, Hybrid) and networking in the cloud by creating and configuring a Virtual Network (VNet) in Microsoft Azure.

In this lab, you will:

- Create a Virtual Network (VNet) and define its address space.
- Configure subnets to segment the network for different services.
- Set up Network Security Groups (NSGs) to secure resources within the VNet.
- Explore routing, and understand how Azure handles traffic between virtual machines and other resources.
- Learn how to connect your VNet to other networks, including on-premises resources, if required.

Whether you're new to Azure or looking to deepen your cloud networking knowledge, this lab will provide you with the practical skills needed to confidently design and manage Azure Virtual Networks.

Let's get started!

Steps for Creating a Virtual Network (VNet):

Step 1: Go to the Azure Portal

•	Open your web browser and go to Azure Portal.

•	Sign in with your Microsoft account (you’ll need an Azure account to proceed; if you don’t have one, you can create a free trial account).

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20Portal.PNG?raw=true)

Step 2: Create a Virtual Network (VNet)

1.	Open the Portal Menu:
   
o	Once you're logged into the Azure Portal, look at the left-hand sidebar.

o	Select "Create a resource"  icon at the top of the page.

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20Create%20a%20resource%20Icon.PNG?raw=true)

2.	Search and Select Virtual Network:
   
o	In the search bar at the top, type "Virtual Network" and click on it when it appears in the list.

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20searchbar.PNG?raw=true)

o	You will be directed to the Virtual Network creation page. Click on the "Virtual network" button. to start the process.

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900VNetworkPage.PNG?raw=true)

o  Then click on "Create"

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900Createbutton.PNG?raw=true)

3.	Configure the VNet Settings: The Create Virtual Network page will appear with several tabs at the top. The tabs you’ll focus on are Basic, Security, IP Addresses, Tags, and Review + Create.
o	Basic Tab: 

 Project Details: 

Subscription: Select your subscription (this is your billing account).

Resource Group: Choose a resource group. You can create a new one or select an existing one. For simplicity, create a new resource group (e.g., "MyResourceGroup").

Instance Details: 

Virtual Network Name: Provide a name for your Virtual Network (e.g., "MyFirstVNet").

Region: Select the region where you want to create the network (e.g., East US, West Europe).

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20VNet%20Create%20Window.PNG?raw=true)

4.	Select the IP Addresses Tab:
   
o	After completing the Basic tab, click on the IP Addresses tab at the top.

o	Default Settings: Leave the default settings for the IP address unless you have a specific IP address range you want to use. By default, Azure will automatically assign an address space (e.g., 10.0.0.0/16).

o	If you'd like to change the IP address, you can do so here.

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20VNET%20Address%20space.PNG?raw=true)

Step 3: Add a Subnet to Your VNet

1.	Add a Subnet:
   
o	Now, click on the "Subnets" section under the IP Addresses tab.

o	Click on the "Add Subnet" button to create a new subnet. 

o  Subnet Name: Give your subnet a name (e.g., "MySubnet").

![Alt text](https://github.com/Kesmondlw79/azurevirtualnetwork4beginners/blob/main/AZ900%20VNET%20Subnet.PNG?raw=true)

o  Subnet Address Range: Choose an IP range within the VNet’s address space (e.g., if your VNet is 10.0.0.0/16, you can create a subnet with 10.0.1.0/24).

o	Once you've entered the details, click "Add" to create the subnet.


 




