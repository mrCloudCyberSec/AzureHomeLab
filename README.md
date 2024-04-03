<h1>Azure Home Lab</h1>

<h2>Business Summary</h2>
Project consists of building a cloud enviornment for learning, experimentation, and honing skill sets based on real-world scenarios within Microsoft Azure. Through out the project, there is an assumption that an active Azure subscription has already been created.
<br />

<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Azure Resources Used</h2>

- <b>Active subscription for Microsoft Azure</b>
- <b>Resource Groups</b>
- <b>Virtual Networks</b>
- <b>Virtual Machines</b>

<h2>Objectives</h2>

- <b>Configuring virtual networks and connect them using peering</b>
- <b>Configure a virtual machine in one of the virtual networks</b>

<h2>Technical Walk-through:</h2>

<h3>Configuring Virtual Networks</h3>

<h4>Creating a Resource Group</h4>

- After logging into Microsoft Azure in portal.azure.com search for "resource group" in the search bar
- Click on "resource group" and click on create at the top left hand corner
- Adding the following details to create a resource group:
  - Subscription being used
  - Name of the resource group being created (the project resource group is named "AzureHomeLab-RG")
  - Select the region for the resource group to be used (the project use the US East region for the AzureHomeLab-RG)
<img src="https://i.imgur.com/hvdPDl6.png">

- Click on "Review + Create" and wait for validation to pass
- Once validation has been passed, click on create and wait for the resource group to deploy.

<h4>Creating a Virtual Network</h4>

- Search for "virtual network" in the Azure portal search bar and click on it
- Click "Create" to start creating a virtual network
- Add the following details in the "Basic tab" of the virtual network creation screen
  - The active subscription being used
  - A resource group to add the virtual network to
  - The name of the virtual network
  - The region to place the virtual network in
<img src="https://i.imgur.com/bwb32dw.png">

- Skip to the IP Addresses tab
- Set a desired IP Address space for the virtual network
<img src="https://i.imgur.com/n3DpDPQ.png">
