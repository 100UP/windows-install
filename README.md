# Guide for Windows Server Installation in KVM

![grafik](https://github.com/100UP/windows-install/assets/57064488/71a3e599-df17-486a-96eb-b301dd2ffb31)

### 1. Reinstall your VPS and select Windows Server 2019

![grafik](https://github.com/100UP/windows-install/assets/57064488/38ef5471-dcfd-48a4-8b47-ea88e131bac1)

### 2. Wait a bit until your VPS is Operational again

### 3. Open the Console

![grafik](https://github.com/100UP/windows-install/assets/57064488/c5170cbc-a6c6-45a9-8639-e483477d5b78)

### 4. Follow through with the Windows installation

![grafik](https://github.com/100UP/windows-install/assets/57064488/98604c32-92c3-49f0-a829-646442eeaa82)

![grafik](https://github.com/100UP/windows-install/assets/57064488/d80728f4-b592-4967-90ca-c43d4f9c58eb)

### 5. If no disk is visible, load the required drivers

![grafik](https://github.com/100UP/windows-install/assets/57064488/23c8fd3b-aa70-4165-bb01-39125245eb47)

![grafik](https://github.com/100UP/windows-install/assets/57064488/a53d039b-07ad-41cd-ba01-ed3b113033f0)

![grafik](https://github.com/100UP/windows-install/assets/57064488/8b722713-735b-485c-b287-a535a43d8d1c)

### 6. Finish the Windows installation

![grafik](https://github.com/100UP/windows-install/assets/57064488/27ccd441-6d2a-4a99-b19e-b9a9f457ed4d)

![grafik](https://github.com/100UP/windows-install/assets/57064488/f3f79efe-79a7-4d2a-b524-45d271ac594b)

Wait for the installation to complete.

### 5. Set a password

![grafik](https://github.com/100UP/windows-install/assets/57064488/dfe984d9-7da4-4d8f-8d92-d090016f8e9a)

### 6. Use the left sidebar to send CTRL + ALT + DEL, then login

![grafik](https://github.com/100UP/windows-install/assets/57064488/7754c01c-4c4d-4f9d-ade8-bbbaf179749a)

### 7. Install required drivers

Start virtio-win-gt-x64 on the CD Drive D:

![grafik](https://github.com/100UP/windows-install/assets/57064488/d3e62ff4-41be-4c21-ae0f-44e4f1bc6420)

Click Next and Install

![grafik](https://github.com/100UP/windows-install/assets/57064488/43485cb3-9a27-4cd3-873a-ab42b47fff71)

Allow NIC Install

![grafik](https://github.com/100UP/windows-install/assets/57064488/7e6cba76-907f-4355-b17d-3051616b848f)

### 8. Also install the guest-agent

Just double click the file

![grafik](https://github.com/100UP/windows-install/assets/57064488/e8244f64-0de1-494c-b3cf-0ecfb8dc6ce3)

### 9. Configure network with a static IP

Click on Ethernet -> Properties -> Internet Protocol Version 4 (TCP/IPv4)  
You can find the IP address and gateways on your VPS IP tab.  
The Subnet mask is always 255.255.255.255 and you can use 8.8.8.8 as DNS server.

![grafik](https://github.com/100UP/windows-install/assets/57064488/9c43f3d0-f365-48ed-9faa-0d1b6979676a)

If you get a warning, confirm it with Yes.

![grafik](https://github.com/100UP/windows-install/assets/57064488/45a47c3a-365f-4353-8265-8bab1e47da6e)

### (Optional) 10. Enable RDP from the internet

![grafik](https://github.com/100UP/windows-install/assets/57064488/e8f46d35-ae9a-47c2-9410-bedd85fd0e06)

Note that this exposes your Windows Server to everyone on the internet!  
You should configure the firewall on the IP tab to restrict access to TCP port 3389 only for Admin IPs.
