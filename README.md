In this lab we will be exploring networking concepts using Azure.

![image](https://github.com/user-attachments/assets/2fb3df61-e38f-41a6-a8db-0d9bc8742c6e)
 - Our first step requires us to create a resource group in our Azure portal using any name you'd like. In this instance, I will be using the name **Wireshark** since we will be using this to explore our networking concepts.

![image](https://github.com/user-attachments/assets/617b38a8-5383-4642-a8c1-03309663b507)
 - Next, we will be creating a Virtual Machine thats located in our created resource group and ran on an image of Windows 10 Pro. (**Be sure to use credentials you will memorize in order to access this VM**)

![image](https://github.com/user-attachments/assets/e97b209d-63d4-48b4-bbcb-239d7273f5c8)
 - Our third step requires us to create another Virtual Machine within the same resource group & virtual network **(Which you can find in the Network settings of the Virtual Machine**) but using the Ubuntu image this time instead of Windows 10 Pro. (**Be sure to use credentials you will memorize in order to access this VM**)

![image](https://github.com/user-attachments/assets/6e4fdb6c-8fe4-4cec-bcc6-6efb288faeee)
 - After both VM's have been created, remotely connect to your Windows 10 Pro VM by copying and pasting it's public IP address and inputting it into your **Remote Desktop Connection** application. (**Your username and password are the created credentials you used to create your VM**)
   <h4>Search > Remote Desktop Connection</h4>

![image](https://github.com/user-attachments/assets/7f361c92-591f-45b6-8099-dbd88c4c1d3f)
 - Once we've remotely connected to the Windows 10 Pro VM, navigate to Wiresharks website and install the Windows x64 Installer version of Wireshark onto the VM's desktop. (https://www.wireshark.org/)

![image](https://github.com/user-attachments/assets/a2f9286d-57af-4e56-b545-972ee510d5d6)
 - When opening Wireshark, make sure to click the blue fin located in the top right corner of the application and filter for icmp traffic.

![image](https://github.com/user-attachments/assets/c9b9a8e1-3b7a-42df-b4e2-2e624e0e577b)
 - Our next step is to open up Powershell within our WiresharkVM and ping our Ubuntu VM to ensure we are getting a response and are on the same virtual network. It should look like the image above.
