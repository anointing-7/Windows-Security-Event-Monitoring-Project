# Phase 2

# Endpoint configuration:
-I created a Windows 10 VM as an endpoint device. I set its preferred DNS to the Server’s IP address. 

- On it, I installed Sysmon for advanced endpoint monitoring.

 <img width="975" height="356" alt="image" src="https://github.com/user-attachments/assets/624a2355-2b96-4d8f-9669-4254ac4991c6" />

-I installed Splunk Universal Forwarder on it. While setting up Splunk Universal Forwarder, I configured the receiving indexer as the Windows server using the server’s IP and used the default port 9997.

<img width="967" height="695" alt="image" src="https://github.com/user-attachments/assets/b4f425bb-5713-482a-b35e-acd3773eda91" />

- I then created an inputs.conf file within the path "C:\Program Files\SplunkUniversalForwarder\etc\system\local", to ensure the right logs were being forwarded to the indexer.
  
- I enabled Windows logging and auditing using the local policy editor.

