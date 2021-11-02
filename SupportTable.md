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
|Spotify|Desktop Client|Spotify|All|Y|N|Y|Spotify desktop client does not work by default with in the absense of IPv4. Web and mobile applications work on IPv6-only. It is possible to run `command`|
|Steam|Desktop Client|Valve|All?|N|N|N|client cannot connect to steam web services over IPv6 (even via NAT64); it will enter offline mode|
|    |   |   |  |  |   |   |    |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|**Hardware**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Fritzbox LTE 6820|FRITZ!OS|AVM|7.27|Y|Y|U|some services are broken/unusable, the basic routing function works|
|Amazon Alexa|Dot|Amazon|N/A|Y|N|Y|This seemed to work with NAT64 in place but as of 11/2/2021 announced an error about not being connected to Wifi when connected to an IPv6 only network|
|Roku|All|Roku|All|N|N|U|Roku has a long tradition of ignoring IPv6 support requests and has no support whatsoever on any of their platforms including the stand alone devices as well as the embedded Roku TVs|
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |    |
|**Service**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Github|Web|Microsoft|All|N|N|Y|Some IPv6 support has been reported. GitHub.IO has v6 support but the main site does not.|
|Twitter|Web|Twitter|All|N|N|Y| |
|    |   |   |  |  |   |   |   |
|---|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |   |
|**Processes**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**NAT64/DNS64 Present**|**Caveats and Notes**|
|Apple recovery boot|MacOSX|Apple|All|U|N|Y|System fails to pull recovery information upon restoration boot while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|Synology initial setup|DSM|Synology|All|U|N|Y|DSM cannot discover setup host while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|    |   |   |  |  |   |   |    |
