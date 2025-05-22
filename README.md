To install WSL on windows10
------------------------------
-->Open powershell : run as administartor
-->Run the below command
  
  dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
  
  TO enable virtualization
  --------------------------
  dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart


"server {
    listen 80;
    server_name cloudlearn.tech;
    location / {
        proxy_pass http://3.109.65.23:3000;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
    }"

