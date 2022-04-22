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

## Note 
* Log Location
  * Log File: C:\Windows\System32\winevt\Logs\Microsoft-Windows-Sysmon%4Operational.evtx
  * Event Viewer: Applications and Services Log > Microsoft > Windows > Sysmon > Operational
* On older systems events are written to the System event log. 
* Event timestamps are in UTC standard time.

## References
* https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon
* https://github.com/SwiftOnSecurity/sysmon-config
* https://github.com/olafhartong/sysmon-modular
* https://github.com/trustedsec/SysmonCommunityGuide
* https://github.com/Neo23x0/sysmon-config