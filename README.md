To install WSL on windows10
------------------------------
-->Open powershell : run as administartor
-->Run the below command
  
  dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
  
  TO enable virtualization
  --------------------------
  dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
