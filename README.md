# Remote-Desktop-using-Powershell-on-windows-10
## How to enable Remote Desktop using Powershell on windows 10 - if Group policy is blocking

# Instructions
Open PowerShell as administrator

Type the following command to enable the remote desktop protocol and press Enter:

  - Set-ItemProperty -Path 'HKLM:\System\CurrentControlSet\Control\Terminal Server' -name "fDenyTSConnections" -value 0

Type the following command to enable remote desktop through the Windows Firewall and press Enter: 

  - Enable-NetFirewallRule -DisplayGroup "Remote Desktop"
