# Task sequence(s)

```
Import-Module "C:\Program Files\Microsoft Deployment Toolkit\bin\MicrosoftDeploymentToolkit.psd1"
New-PSDrive -Name "DS001" -PSProvider MDTProvider -Root "C:\DeploymentShare"
import-mdttasksequence -path "DS001:\Task Sequences" -Name "Windows 10 Pro Dutch" -Template "Client.xml" -Comments "" -ID "WIN10PD" -Version "1.0" -OperatingSystemPath "DS001:\Operating Systems\Windows 10 Pro in Windows 10 Pro DUTCH x64 install.wim" -FullName "Guillermo" -OrgName "Guillermo.inc" -HomePage "about:blank" -Verbose
```