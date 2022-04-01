## ***"IPv6-only" is defined as the ability to function at full capacity with all features in the complete absense of legacy IPv4. For some entries, this may mean that they exist as dual stack but have 100% functionality from a client or peer that has no legacy IPv4.***

## Legend:
### Y: Yes

### N: No

### U: Unknown  


|    |   |   |  |  |   |   |    |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|**Software**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|    |   |   |  |  |   |   |    |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|Spotify|Desktop Client|Spotify|All|Y|N|Y|Spotify desktop client does not work by default with in the absense of IPv4. Web and mobile applications work on IPv6-only. It is possible to run the command-line switch `--experimental-network` and make the platform work as v6-only|
|Steam|Desktop Client|Valve|All?|N|N|N|client cannot connect to steam web services over IPv6 (even via NAT64); it will enter offline mode|
|Epic Games Launcher|Desktop Client|Epic|All?|N|N|N|client cannot connect to epic web services over IPv6 (even via NAT64)|
|Rockstar Games Launcher|Desktop Client|Rockstar Games|All?|N|N|N|client cannot connect to web services over IPv6 (even via NAT64)|
|Unifi controller|All|Ubiquity|All|N|N|Y|underlying operating system may support IPv6 (or IPv6 only) but the unifi controller software does not support any functionality over IPv6, including discovery or management of any devices| 
|AnyDesk|Desktop Client|AnyDesk|All?|N|N|U|client does not work over IPv6-only (may via NAT64)|
|    |   |   |  |  |   |   |    |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|**Hardware**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Fritzbox LTE 6820|FRITZ!OS|AVM|7.27|Y|Y|U|some services are broken/unusable, the basic routing function works|
|Amazon Alexa|Dot|Amazon|N/A|Y|N|Y|This seemed to work with NAT64 in place but as of 11/2/2021 announced an error about not being connected to Wifi when connected to an IPv6 only network|
|Roku|All|Roku|All|N|N|U|Roku has a long tradition of ignoring IPv6 support requests and has no support whatsoever on any of their platforms including the stand alone devices as well as the embedded Roku TVs|
|Unifi|All|Ubiquity|All|Y|N|Y|Most unifi hardware supports receiving an IPv6 address via SLAAC, or manually assigning it via the SSH terminal. Devices will not use these addresses for management, logging, or discovery via the Unifi software. It may log to a remote syslog server over IPv6 adn will listen to SSH via IPv6|
|Strata SD-WAN|PAN-OS|Palo Alto|10.1|N|N|N|Palo Alto Strata SD-WAN has no IPv6 support|
|SD-WAN (Viptela, not Miraki)|vMangae/vBond/vSmart/vEdge/cEdge|Cisco|20.6|Y|N|N|Control connections between vManage/vBond/vSmart works IPv6 only. vManage web page access works IPv6 only in theory, but [CSCvz60689](https://bst.cloudapps.cisco.com/bugsearch/bug/CSCvz60689) prevents logins via IPv6. Tunnels are IPv4 only but can transport IPv6.|
|SD-WAN|VOS|Versa Networks|21.2|Y|N|N|Tunnels work IPv6 only. Control connections between Director and Controller are IPv4 only. Director does not Support IPv6.|
|    |   |   |  |  |   |   |    |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|**Service**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Github|Web|Microsoft|All|N|N|Y|Some IPv6 support has been reported. GitHub.IO has v6 support but the main site does not.|
|Twitter|Web|Twitter|All|N|N|Y| |
|Plex|Web|Plex.tv|All|N|N|Y|Plex has "partial" support. Plex supports IPv6 at the socket-layer, but doesn't "auto-configure" IPv6 on the remote-end (the [ipv4].[server-uid].plex.direct system), as such, doscovery via IPv6 does not work at all unless a manual hostname is created and appropriate DNS entries for it (which are sent up to plex.tv as additional hostnames to try)|
|Synology|Synology Cloud|Synology|All?|N|N|Y|Service does not work over IPv6-only (may via NAT64)|
|    |   |   |  |  |   |   |   |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |   |
|**Processes**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Apple recovery boot|MacOSX|Apple|All|U|N|Y|System fails to pull recovery information upon restoration boot while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|Synology initial setup|DSM|Synology|All|U|N|Y|DSM cannot discover setup host while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|    |   |   |  |  |   |   |    |
