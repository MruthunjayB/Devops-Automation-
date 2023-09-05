nptserver Playbook
=================
The ansbile playbook is intended to be used on a node to set the ntpserver , as per the requirement passed in command line 
------------
- `operating system` - Works for both Windows/RHEL OS and set ntp servers as passed ( if only Primary NTP is passed then only primary NTP is set )
=========
The following platforms are tested. - windows 2016 & 2019
- RHEL 7 & 8 Attributes
----------
Key | Type | Description | Default
--- | ---- |------------ |--------
[:cmsng][:ntpserver][:primary] |String |attribute provides the primary ntp server ip to be set on the newly provisioned vm
[:cmsng][:ntpserver][:secondary] | String | provides the secondary ntp server ip to be set on the newly provisioned vm

Note: Secondary NTP value is always optional in case of both Linux / Windows and sets only mandatory primary NTP ip if secondary NTP is not parsed.