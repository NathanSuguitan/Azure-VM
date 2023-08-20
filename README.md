<p align="center">
  
![microsoft-azure-virtual-machine-blu-cirrus-business-cloud-services-montreal-quebec-canada-1024x460](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/44c7ac21-17ba-4de3-9834-138a2d656b3d)

</p>

<h1>Azure VM - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and deployment of an Azure Virtual Machine (VM).<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Account (create your free account <a href="https://azure.microsoft.com/en-us/free/search/?ef_id=_k_Cj0KCQjw0IGnBhDUARIsAMwFDLkdUQC7p5LbZsFOjKsEkUjWR2TwopCr0I1iHxT3yTWBCUmxX5lQTyYaAkD9EALw_wcB_k_&OCID=AIDcmmfq865whp_SEM__k_Cj0KCQjw0IGnBhDUARIsAMwFDLkdUQC7p5LbZsFOjKsEkUjWR2TwopCr0I1iHxT3yTWBCUmxX5lQTyYaAkD9EALw_wcB_k_&gad=1&gclid=Cj0KCQjw0IGnBhDUARIsAMwFDLkdUQC7p5LbZsFOjKsEkUjWR2TwopCr0I1iHxT3yTWBCUmxX5lQTyYaAkD9EALw_wcB">here</a>)
- <a href="https://github.com/NathanSuguitan/Azure-ResourceGroups">Resource Group</a> deployed within Azure
- A <a href="https://apps.apple.com/app/microsoft-remote-desktop/id1295203466?mt=12">Remote Desktop Client</a> for macOS users

<h2>Deployment Steps</h2>

1. Sign in to the [Azure portal](https://portal.azure.com).
2. Create a <a href="https://github.com/NathanSuguitan/Azure-ResourceGroups">resource group</a>
3. After the resource group has been successfully deployed, enter **virtual machines** in the search
4. Under **services**, select **virtual machines**

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/a38d6f5a-02ac-44bf-a498-4e0dee2a81bd)

5. In the **virtual machines** page select **create**, then select **azure virtual machines**
6. Under **project details** in the **resource groups** drop down select your **resource group**
7. Under **instance details** enter a name for **Virtual machine name**, select the same **region** as your resource group, and choose **Windows 10 Pro, version 22H2 - x64 Gen2** for your image. Leave all other options as default

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/bad67d68-95da-490e-af00-43bb2d616afc)

8. Under **Administrator Account** add a username and password
9. Leave all other options as dafault
10. Under **Licensing** check the box to confirm hosting rights

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/ea05136e-ef6c-4c05-9004-4cf0c27eb2f5)

11. Select **review + create**

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/a0658c7f-1ac7-4210-8b9e-6625a51de584)

12. After validation passes, select **Create** at the bottom of the page

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/e848e9c3-f007-4fec-bae6-41234e297da6)

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/9d12e2b1-ba8a-4c2a-9ad3-275ba60b6198)

13. After deployment, select **Go to resource**

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/f591a1ed-6668-4ef3-a87d-bb5628d947ca)

## Connect to Virtual Machine

Create a remote desktop connection to the virtual machine.

This portion of the tutorial will outline how to connect to your VM from a Windows computer. On a Mac, you need an RDP client such as this <a href="https://apps.apple.com/app/microsoft-remote-desktop/id1295203466?mt=12">Remote Desktop Client</a> from the Mac App Store.

1. Under **essentials** copy your public IP address

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/247b1c55-f53c-4f43-8c4d-4c2cb83c8216)

2. Press the windows key and search **remote desktop connection**. Select Remote Desktop Connection

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/b1a5c02b-b7c5-4016-a7a8-c8a5c300e49b)

3. In the Remote Desktop Connection, enter the public IP address of the VM, and enter the username and password

![image](https://github.com/NathanSuguitan/Azure-VM/assets/138082246/dc915d0b-b4c6-4340-a78d-c814711160d9)

## Clean up resources
When no longer needed, you can delete the resource group, virtual machine, and all related resources.

1. On the Overview page for the VM, select the Resource group link.
2. At the top of the page for the resource group, select Delete resource group.
3. A page will open warning you that you are about to delete resources. Type the name of the resource group and select Delete to finish deleting the resources and the resource group.
