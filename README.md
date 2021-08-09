# sysmon-config
Sysmon configuration file

## Required
* Windows OS
* Sysmon version 13 or higher

## Use
run cmd as administrator
1. Install 
    ```
    sysmon.exe -accepteula -i sysmonconfig-export.xml
    ```
1. Update config 
    ```
    sysmon.exe -c sysmonconfig-export.xml
    ```
1. Uninstall
    ```
    sysmon.exe -u
    ```
1. Log Location
    * Microsoft-Windows-Sysmon/Operational
