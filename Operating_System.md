# Operating System

### Windows 10 DUTCH x64

```
Import-Module "C:\Program Files\Microsoft Deployment Toolkit\bin\MicrosoftDeploymentToolkit.psd1"
New-PSDrive -Name "DS001" -PSProvider MDTProvider -Root "C:\DeploymentShare"
import-mdtoperatingsystem -path "DS001:\Operating Systems" -SourcePath "C:\DeploymentShare\Windows ISO unpacked\Windows_10_DUTCH" -DestinationFolder "Windows 10 Pro DUTCH x64" -Move -Verbose
```