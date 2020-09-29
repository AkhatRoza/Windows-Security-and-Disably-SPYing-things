# Windows-Security-and-Disably-SPYing-things
If you are using the Windows you can disable a lot of unnecessary services on your OS 
bat file contains main spy services of Windows but can disabel by your taste 

Before you start with all manipulations nake backup 
reg export HKLM hklm_backup.reg

**net stop dmwappushservice 
sc config dmwappushservice start=disabled
net stop diagnosticshub.standardcollector.service
sc config diagnosticshub.standardcollector.service start=disabled
net stop DcpSvc
sc config DcpSvc start=disabled
net stop WerSvc
sc config WerSvc start=disabled
net stop PcaSvc
sc config PcaSvc start=disabled
net stop DoSvc
sc config DoSvc start=disabled
net stop WMPNetworkSvc
sc config WMPNetworkSvc start=disabled
net stop RemoteRegistry
sc config RemoteRegistry start=disabled
net stop TermService
sc config TermService start=disabled
net stop TrkWks
sc config TrkWks start=disabled
net stop DPS
sc config DPS start=disabled
pause 


**disable xbox services that to increase CPU power if you are using them then no need

net stop XblAuthManager
sc config XblAuthManager start=disabled
net stop XblGameSave
sc config XblGameSave start=disabled
net stop XboxNetApiSvc
pause


sc config XboxNetApiSvc start=disabled
