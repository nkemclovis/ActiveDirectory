# Creating and Configuring Active Directory on Windows 2019 Server using Virtual Box

<p>Overview:</p>
<p> In this project, I will download and install oracle virtualbox which will be used to run our virtual machines. After that’s installed, I will download a Windows 10 and a Windows 2019 Server ISO which I’m going to use to install the two operating systems on two separate virtual machines. Next after I have downloaded and install everything, I’m going to create the first virtual machine which is going to be the domain controller to house the active directory,  this virtual machine will have  two network adapters one of which will be used to connect to the internet and the other will be used to connect to the virtual box internal private network that the client machine will be connected to. After the virtual machine is created, I’m going to install server 2019 on it and assign IP addresses for the internal network. The external network will automatically get IP addresses from the home network (home router). With the IP addresses setup, I’m going to name the server,  install an active directory and create the domain. Then I’m going to configure NAT and RAS so the client on the private network can reach the internet through the domain controller. Next I will set up a DHCP on the domain controller so when the windows 10 machine can automatically get an IP address. The last thing I will do on the domain controller before creating the client virtual machine will be to run a powershell script that will automatically create a thousand users in the active directory.
Finally I will create another virtual machine and install windows 10 on it and this virtual machine will be connected to the private virtual network, it will be named client1 and join it to the domain where I can use one of the domain accounts created to log into it.</p>

- [Active Directory Project](https://drive.google.com/file/d/1f0NZjgwC0ps9oxqn98KcgvgMZ3Ce_mi2/view?usp=sharing)
