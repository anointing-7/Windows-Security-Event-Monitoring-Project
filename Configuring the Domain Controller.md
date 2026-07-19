# Windows Server Setup:
-I set up a Windows Server 2022 version using Oracle VirtualBox.
-By selecting the option to create a new virtual machine, giving the new VM a name, selecting the right ISO image file, and manually assigning resources, I was able to get my Windows Server VM up and running.
-During the Server OS setup, I selected the Datacenter Desktop Experience version.
-I set up a strong admin password (Insert screenshot).
-I assigned a static IP address to the server.

<img width="975" height="502" alt="image" src="https://github.com/user-attachments/assets/756e8dc4-6583-4dda-9d2f-05d05064b0ff" />

 
-I created a local domain and set up Active Directory  in PowerShell using the command: Install-Windows Feature AD-Domain-Services -IncludeManagementTools , so I could connect an endpoint device to the domain, thereby converting the server into a Domain Controller.

 <img width="975" height="394" alt="image" src="https://github.com/user-attachments/assets/4a6bf1bd-c4f8-4290-be3b-662bce366afa" />


-I enabled Windows logging and auditing using the local policy editor.

 <img width="975" height="734" alt="image" src="https://github.com/user-attachments/assets/6941ee4e-32b3-442c-873f-2e88b3f850cc" />


### Challenges experienced:
-	I selected the standard version at first, and that gave me a terminal-based system, so I restarted the process of setting up the VM, and selected the Datacenter Desktop Experience version which worked fine.
-	After setting the static IP, I had issues connecting to the internet. I did some troubleshooting and realized it was a DNS-related issue, and set the preferred DNS to 8.8.8.8, which resolved the issue.



