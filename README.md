<h1>Azure Home Lab</h1>

<h2>Business Summary</h2>
Project consists of building a cloud enviornment for learning, experimentation, and honing skill sets based on real-world scenarios within Microsoft Azure. Through out the project, there is an assumption that an active Azure subscription has been created.
<br />

<h2>Objectives</h2>

- <b>Configuring virtual networks and connect them via peering</b>
- <b>Configure a virtual machine for two of the virtual networks</b>
- <b>Secure the perimeter of the Azure Cloud enviornment</b>

<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Azure Resources Used</h2>

- <b>Active subscription for Microsoft Azure</b>
- <b>Resource Groups</b>
- <b>Virtual Networks</b>
- <b>Virtual Machines</b>

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

- Keep the default settings in the "Security" tab and skip to the "IP Address" tab
- Set a desired IP Address space for the virtual network
<img src="https://i.imgur.com/n3DpDPQ.png">

<h5>Creating a Virtual Network subnet</h5>

- Click on "Add a subnet" and the side window would appear to create a subnet
- Adding the following details to the subnet:
  - Subnet purpose: Default
  - The name of the subnet
  - Set the desired starting IP address for the subnet
  - Set the desired size (subnet mask) for the subnet
  - Keep all other settings as the default setting
  - Click "Add" at the bottom of the side window to finish
<img src="https://i.imgur.com/yyRhGGK.png">

- The "IP Addresses" tab should look similar to the example below:
<img src="https://i.imgur.com/UbkXies.png">

- Click on the "Review + Create" and let validation pass
- After validation has passed, click "Create" to deploy the virtual network

- Repeat the previous steps to create more virtual networks and subnets with a different name for each of the new virtual networks and subnets
