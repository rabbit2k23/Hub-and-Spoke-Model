**Connect Hub and Spoke Networks with VNet Peering**


1> Having Two Virtual network Hub Vnet and Spoke Vnet
2> Hub Vnet is having App Server and Spoke Vnet is having Jump Server.
3> Remote access to Jump server and from jump server perform RDP to app server privately using Vnet Peering.

 Diagram
![alt text](image.png)


Create and associate public IP to Jump server Nic to get remote access.

![alt text](image-1.png)

![alt text](image-2.png)

![alt text](image-3.png)

Create Peering between hub and spoke Vnets

![alt text](image-4.png)

![alt text](image-5.png)

![alt text](image-6.png)

![alt text](image-7.png)

Added Inbound NSG rule on SpokeVnet for RDP on Jump server.

![alt text](image-8.png)

Add Inbound NSG rule on HUB-Vnet NSG to connect Jump server to App server.

![alt text](image-9.png)

Logged in to the Jump server and then do RDP to App server.

![alt text](image-10.png)

![alt text](image-11.png)
