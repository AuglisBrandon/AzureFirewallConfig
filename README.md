<h1>AzureFirewallConfig</h1>

<h2>Description</h2>
Azure tutorial on how to configure their firewall services by hands on demonstration. The step by step process will include, creating a resource group, VN, VM, Firewall, route tables, and rules on said firewall
<br />


<h2>Languages and Utilities Used</h2>

- N/A

<h2>Environments Used </h2>

- <b>Microsoft Azure Cloud (Free Trial or Pay as you Go)</b>
- <b>Azure VM</b>
- <b>Resource Group</b>
- <b>Virtual Network</b>

<h2>Walk-through: (Note: This requires you to have made an Azure Free Trial account or Pay as you Go account)</h2>

<p align="center">
Step by Step process for this lab: <br/>
<br/>
<br/>

- We will first create a Resource Group. So in the search bar type in "Resource Group" and open it. Then click "Create" <br/>
![Screenshot 2022-10-06 044046](https://user-images.githubusercontent.com/114842751/194247626-b3ff2951-3bd4-48be-a9ba-e7f06ea0e2e9.png)
<br/>
<br/>

- Next you will name your Resource Group, and everything else just leave as is, then click "Review + create" then "Create": <br/>
![Screenshot 2022-10-06 044839](https://user-images.githubusercontent.com/114842751/194248487-9694cc95-a4c3-4bf2-97e6-9bf019b137d6.png)
<br/>
<br/>

- Now that the Resource Group has been created we will move on to creating the Virtual Network. So in the search bar look up Virtual Network and once there click, "Create": <br/>
![Screenshot 2022-10-06 045346](https://user-images.githubusercontent.com/114842751/194249614-fd82e41f-449f-4a5e-a29d-848d8fccb221.png)
<br/>
<br/>

- Once in, if the Resource Group hasnt automatically selected the group that you created then press the arrow key and select it. Afterward you need to name your Vritual Network. Afterwards click "IP addresses" at the top: <br/>
![Screenshot 2022-10-06 045713](https://user-images.githubusercontent.com/114842751/194251727-c27133cf-878e-45b1-b7c3-88da4a45b305.png)

- *Note: Feel free to change the Region to whatever suits your needs.*
<br/>
<br/>

- Once in IP Addresses, click "Add an IP address space" and fill in the following: <br/>
![Screenshot 2022-10-06 050537](https://user-images.githubusercontent.com/114842751/194256675-d636b25f-6177-4764-8990-ac2300a48ff9.png)
<br/>
<br/>

- Next we need to add some subnets to our new IP Address, so click "Add a subnet" and then fill in the following then click "Add": <br/>
![Screenshot 2022-10-06 051041](https://user-images.githubusercontent.com/114842751/194258017-078493c5-9195-4818-b659-764976073b89.png)
<br/>
<br/>

- We will create one more following the same steps as before and then after go to Review and Create and then click "Create" after validation: <br/>
![Screenshot 2022-10-06 051252](https://user-images.githubusercontent.com/114842751/194270226-7998ee41-df38-4fb5-b7ec-03d2504d069d.png)


*Note: Security and Tags will be left as is.*
<br/>
<br/>

- If you go back to Resource Group and click "Overview" and then "Topology" you will see the network you have just created: <br/>
![Screenshot 2022-10-06 051904](https://user-images.githubusercontent.com/114842751/194259934-ca2b95b3-732e-4051-8132-aa3fe46a5fdd.png)
<br/>
<br/>

- Next we will be creating the Virtual Machine. So Type in the search bar "Virtual machine" and go to that page. Once there, at the left hand corner click "Create".
<br/>
<br/>

- From here to keep it simple, I will fill in the following and just follow along(Keep in mind that the region needs to be set to your region i.e. West to West etc.)<br/>
![Screenshot 2022-10-06 052712](https://user-images.githubusercontent.com/114842751/194261800-b687201a-3979-4e85-abc2-7872951d336b.png)
![Screenshot 2022-10-06 052736](https://user-images.githubusercontent.com/114842751/194261924-dd425712-2cf3-41c6-8b33-fc4eb0f67c81.png)
*Name your username something other than mine*
![Screenshot 2022-10-06 052907](https://user-images.githubusercontent.com/114842751/194262262-c125de82-808c-4206-84e4-76c9fee0bdec.png)
![Screenshot 2022-10-06 053946](https://user-images.githubusercontent.com/114842751/194264650-da52a8dd-d923-47b0-8734-d0471ab848b8.png)
![Screenshot 2022-10-06 054048](https://user-images.githubusercontent.com/114842751/194264838-2b53d701-8d7a-43d8-b924-d8c6549f3b5a.png)
![Screenshot 2022-10-06 054124](https://user-images.githubusercontent.com/114842751/194264983-83b2feaa-e98b-4cf6-ac32-4a43dee51848.png)
![Screenshot 2022-10-06 054155](https://user-images.githubusercontent.com/114842751/194265124-243cabbe-c80d-473b-b6ec-60f28b685ceb.png)
![Screenshot 2022-10-06 054220](https://user-images.githubusercontent.com/114842751/194265203-a19ad397-c414-40c0-921a-57513b7fbb5b.png)
![Screenshot 2022-10-06 054253](https://user-images.githubusercontent.com/114842751/194265354-fe89da66-adf7-4bd1-8e66-67bbc613a4bc.png)

*Note: I know most of these are blank however, I think its better to see that they are left blank than guess if it is or not.*
<br/>
<br/>

- After you have set up everything as instructed click "Create" and go to "Resource Group" and then the VM. <br/>
<br/>
<br/>

- As you will see there is no Public IP Address. Next we need to go to Networking so click on "Networking" on the left hand side: <br/>
![Screenshot 2022-10-06 060419](https://user-images.githubusercontent.com/114842751/194271826-1b4a3ff5-14f1-4abf-8f8b-62fdc23aed03.png)
<br/>
<br/>

- Then click on the highlighted part of "Network Interface": <br/>
![Screenshot 2022-10-06 060544](https://user-images.githubusercontent.com/114842751/194273329-e0408a0c-bb99-429a-9234-638470e7add9.png)
<br/>
<br/>

- Next click "IP Configuration" then select the IP Address you created: <br/>
![Screenshot 2022-10-06 064548](https://user-images.githubusercontent.com/114842751/194281771-6d41622c-ec85-42d5-bf16-94f25048e63f.png)
<br/>
<br/>

- Swith from Dynamic to "Static" then Save: <br/>
![Screenshot 2022-10-06 064759](https://user-images.githubusercontent.com/114842751/194282300-3f8ada75-9127-45fb-ac3c-3c504a13fc50.png)
<br/>
<br/>

- Now before we continue to creating the firewall go back to "Resource Groups" and then go to the VNet that we created -> Then click on "Subnets" on the left panel -> We need to delete Subnet 2 (Made a mistake for future steps however, I wanted to keep it in for reference plus its good practice) -> Then click on the "+ Subnet" to create a new one -> Then name the subnet "AzureFirewallSubnet" -> Set the range to "192.168.2.0/24" -> Then click "Save" at the bottom. <br/>
<br/>
<br/>

- Now go to the search bar and type "Firewall" then go to the Firewall page. Once there click "Create", now fill in the following: <br/>
![Screenshot 2022-10-06 070748](https://user-images.githubusercontent.com/114842751/194286477-4284a129-a314-48d2-8b40-b3091d196e04.png)
![Screenshot 2022-10-06 070807](https://user-images.githubusercontent.com/114842751/194286489-0844dd3e-581c-4745-947e-82f423d368cd.png)
<br/>
<br/>

- Now click "Add new" where it says Public IP address: <br/>
![Screenshot 2022-10-06 070922](https://user-images.githubusercontent.com/114842751/194286729-0d7d30a1-4ef1-41e3-b6cc-1b15ab0a02eb.png)
<br/>
<br/>

- Fill in the following then click "Ok", then click "Review + Create" then then "Create": <br/>
![Screenshot 2022-10-06 071026](https://user-images.githubusercontent.com/114842751/194287013-d8b868bb-fbd2-477a-981d-deac455eac06.png)
<br/>
<br/>

- Once the Firewall has deployed, click "Resource group" and then click "Rules(classic)" in the left hand panel: <br/>
![Screenshot 2022-10-06 071828](https://user-images.githubusercontent.com/114842751/194288695-8afe43f4-1448-4c25-bdb8-366c56ae793b.png)
<br/>
<br/>


- Next click "Add NAT rule collection" and fill in the following: <br/>
![Screenshot 2022-10-06 072607](https://user-images.githubusercontent.com/114842751/194290221-2b59843c-5c63-4cf9-b8d7-bcd4b794a249.png)
![Screenshot 2022-10-06 072617](https://user-images.githubusercontent.com/114842751/194290233-b77ebd28-aaca-4f76-81d2-e3f6e6d5992e.png)
<br/>

- *Note: the Destination Ports is your Firewall Public IP, do not copy mine or you will not have properly working destination port.* <br/>
<br/>
<br/>

- Click "Add" and wait for your NAT rule to update. (May need to refresh) <br/>
![Screenshot 2022-10-06 073048](https://user-images.githubusercontent.com/114842751/194291170-1d9f73d4-1ff4-4c89-ab1a-68f69e49c570.png)
<br/>
<br/>

- Next we need to use Remote Desktop Connection so that we can login to our VM. The steps are as follows: Open Remote Desktop Connection on your private pc -> When the window pops up in Computer type in the Public IP Address and then press "Connect" -> You will be prompted to fill in the Admin login and Password you created in the beginning -> This will start the VM. <br/>
<br/>
- *Note: If you come across an error double check your NAT rule and check that the destination ports is the Public IP Address and the translated address is the Private IP of the VM.* <br/>
<br/>
<br/>

-So now that we are logged into the Server we created, click on "Local Server" in the top left hand corner. Then click "IE Enhanced Security Configuration" and turn off Users then click "Ok": <br/>
![Screenshot 2022-10-06 075238](https://user-images.githubusercontent.com/114842751/194295246-18f544ed-f99b-4c5a-a669-5be4af777f5c.png)
<br/>
<br/>

- Next open up Internet Explorer, you will be welcomed with a prompt. Leave everything as is and click "Ok". <br/>
<br/>
<br/>

- You now have access to the internet through your server and the firewall you have created! <br/>
<br/>
<br/>

- The next step is to add the Route Table. So now going back to Azure, in the search bar type "Route Tables" and go to the page. Click "Create route table": <br/>
![Screenshot 2022-10-06 075946](https://user-images.githubusercontent.com/114842751/194296491-0c7503bf-166e-4ff8-ac05-1cfedf3afddb.png)
<br/>
<br/>

- Fill in the Following then click "Review + create" then "Create". <br/>
<br/>
<br/>

- Next click "Go to resource". From here on the left hand panel click on "Routes". Click "Add" then fill in the following then click "Add": <br/>
![Screenshot 2022-10-06 080635](https://user-images.githubusercontent.com/114842751/194297805-8c5fbb6b-86f5-43b2-a379-00f269728759.png)
<br/>
<br/>

- Next go to "Subnets" then click "Associate": <br/>
![Screenshot 2022-10-06 080859](https://user-images.githubusercontent.com/114842751/194298142-43ca0410-cc36-49d4-9f94-54a6d12ef17a.png)
<br/>
<br/>

- Fill in the Following then click "Ok": <br/>
![Screenshot 2022-10-06 081027](https://user-images.githubusercontent.com/114842751/194298462-9d72fdca-3d08-4b69-9f21-4348600c78b9.png)
<br/>
<br/>

- Now going back to the VM and now go and try and  pull up google.com. You will notice you have lost connection and will eventually timeout. <br/>
![Screenshot 2022-10-06 081422](https://user-images.githubusercontent.com/114842751/194299049-939b7cc7-a54a-4b29-ae2d-5be7505dce25.png)
<br/>
- *Note: The reason is because we set up the route table that now created essentially rules on inbound traffic*
<br/>
<br/>

- Now going back to Azure again, go to Firewalls and then back to Rules(classic). Now we need to add an Application Rule. <br/>
![Screenshot 2022-10-06 081954](https://user-images.githubusercontent.com/114842751/194299951-ea1a52e7-43d6-4b1f-97a9-6fae649da5f2.png)
<br/>
<br/>

- Fill in the following then click "Add": <br/>
![Screenshot 2022-10-06 082150](https://user-images.githubusercontent.com/114842751/194300383-42277c95-20fc-4ccb-9b69-2b35f10d9607.png)
<br/>
<br/>

- *Note: What we did just now was create an application rule that now allows google.com by updating the firewall.* <br/>
<br/>
<br/>

- CONGRATULATIONS! You just created a Firewall within a virtual network and Windows Server 2022 VM! <br/>
<br/>
- Make sure to delete the resource group so you do not get charged or go through your Azure Free credit.
