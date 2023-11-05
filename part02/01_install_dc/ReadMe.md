# 01 Installing the Domain Controller

1. Use 'sconfig; to :
   - Change the hostname
   - Chnage the IP address to static
   - Change the DNS server to our own IP address

2. Install the Active Directory Windows Feature

```shell
Install-WindowsFeature AD-Domain-Services -IncludemanagementTools
import-Module ADDSDeployment
Install-ADDSForest
```
- Enter your Domain name: xyz.com
- Set password
- The System will restart

