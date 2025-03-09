<p align="center">
<img src="https://i.imgur.com/4wqxHID.png" height="40%" width="60%" alt="Microsoft Azure Logo"/>
</p>

<h1 align="center">VPN Setup and Geo-Location Testing</h1>

In this lab, you will set up a virtual machine in Azure, test internet geolocation from different regions, and configure a VPN to explore how it affects online location and browsing experiences. You will also learn to manage Azure resources and observe the impact of VPN connections on websites and services.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/03e61f89-4a6e-4ba2-83eb-59539d1b91fe">

<h1 align="center">Lab Overiew</h1>

*Image Above Explained*

1. Visit https:whatismyipaddress.com from your personal computer
2. Create a VM and connect via RDP
3. Access https:whatismyipaddress.com from the VM
4. Install and connect to a VPN on the VM
5. Revisit https:whatismyipaddress.com from the VPN

<h1 align="center">What is a VPN?</h1>

A **VPN (Virtual Private Network)** is a secure connection that encrypts your internet traffic and routes it through a server in another location, masking your IP address and making your online activities more private.  

**Example:** If you're in the U.S. and connect to a VPN server in Japan, websites will see your location as Japan, allowing access to region-specific content while keeping your data secure.

**VPN Metaphor Example:** A VPN is like a secure tunnel for your internet traffic. Imagine sending a letter through a courier that hides the sender’s address and replaces it with their own. The recipient sees the courier's address, not yours, keeping your identity private and secure.

## Environment and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- ProtonVPN
- WhatIsMyIpAddress.com

## Operating systems Used

- Windows 10 (21H2)

## High-Level VPN Setup and Geo-Location Testing Steps

- Browse https:whatismyipaddress.com from your Personal Computer
- Browse https:whatismyipaddress.com from your Virtual Machine
- Install and connect to a VPN on the VM
- Revisit https:whatismyipaddress.com from the VPN
- Explore websites using a VPN on the VM

## Configuration Steps

<details>

<summary>

### 🌐 Step 1: Browse https:whatismyipaddress.com from your Personal Computer

</summary>

Before creating our resources we'll **browse to https:whatismyipaddress.com** from our **personal computer** and take note of this in a text file.

*This is number 1 from the lab overview image explanation.*

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/75a13f40-051d-47c1-8940-6dfeae85bbfe">

</details>

<details>

<summary>

### 🌐 Step 2: Browse https:whatismyipaddress.com from your Virtual Machine

</summary>

Create your resource group and virtual machine then login. **Pick a different region** from your own.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/b5fd3801-609c-45ce-bd2f-d844a62323ea">

<br>
<br>
<br>

Once inside the VM open Microsoft Edge and **browose https:whatismyipaddress.com** then **take note** of it in a text file.

*This is number 3 from the lab overview image explanation.*

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/29ff42dd-d76a-424f-9516-0f6dafc2bcbd">

</details>

<details>

<summary>

### 🌐 Step 3: Sign Up for ProtonVPN and Test the VPN Connection on the VM

</summary>

Once you create an account login on your VM and go to **Downloads**, select **Windows**, then on the next page select **Windows 11/10**.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/3f4f9931-726d-43fb-afd8-2c620c0d1e28">

<br>
<br>
<br>

Open the **ProtonVPN download**, click **OK**, click **Next**, click **Install**, then **login**.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/d1de5592-3da7-4281-af35-217d33dafeeb">

<br>
<br>
<br>

Once you get logged in select **Quick Connect** in the upper left corner and ProtonVPN will assign your VM a VPN server in a new region.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/dc981896-b266-4617-93f1-aeacc2fe8b55">

</details>

<details>

<summary>

### 🌐 Step 4: Revisit https:whatismyipaddress.com from the VPN

</summary>

Now that you have a VPN linked to your VM you can **Revisit https:whatismyipaddress.com** and **take note** of the new information in a text file.

Observe in the text file how each piece of information is different, highlighting the difference between using a VPN and not using one. A **VPN will help mask your true IP address** and **encrypt your internet traffic**, making it significantly harder for malicious actors to track your online activity, access your personal or business information and resources, or even launch targeted attacks based on your location.

*This is number 5 from the lab overview image explanation.*

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/7df18a65-14e9-4e01-8f54-0381a52cc762">

</details>

<details>

<summary>

### 🌐 Step 5: Explore Websites using a VPN on the VM

</summary>

**Visit Google** and **perform a search**. Observe how the search results populate, as the language and content may reflect the region of your current IP address or VPN connection.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/0efc13bd-3639-486d-80c1-f9ef5369cbeb">

<br>
<br>
<br>

Change your server and we'll try another website next. Select **Change Server** in the upper left corner.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/59f7b67e-0baf-4049-93b4-241e8710b73a">

<br>
<br>
<br>

**Browse samsung.com, apple.com, or youtube.com** and notice the region your VPN is in will be displayed as the location on the website.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/b4e8f855-68d6-4777-9e74-af59c1e1619e">

</details>

<details>

<summary>

### 🌐 Step 5: Clean Up Azure Resources

</summary>

Go back into your Azure portal and **delete all your resources** when your done.

<img width="800" alt="isolated" src="https://github.com/user-attachments/assets/42d9237b-d1ab-498f-a3e0-fca36ea63be5">

</details>

<h2 align="center">Final Thoughts</h2>

This lab demonstrated how VPNs can enhance online privacy, mask your location, and provide access to region-specific content. By setting up a virtual machine in Azure and testing a VPN, we explored the practical impacts of geolocation changes and gained hands-on experience with cloud resources and VPN configuration. These skills are essential for understanding network security, privacy, and global connectivity in today’s digital world.

If you haven’t done so yet, check out my other labs to further enhance your knowledge and skills. Explore topics like [Group Policy and Account Management](https://github.com/vincentchachere/Group-Policy-and-Managing-Accounts), [File Shares and Permissions](https://github.com/vincentchachere/Network-File-Shares-and-Permissions), and [DNS Resolution](https://github.com/vincentchachere/DNS-Fundamentals).

Thank you for following along with this project. Your time and effort in learning and implementing these concepts are greatly appreciated. 

☎️ For questions or to connect you can reach me at: www.linkedin.com/in/vincentchachere
