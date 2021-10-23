# Broken IPv6-only
## A running list of applications and processes that just do not work with the total absence of IPv4 on on a host. Contributions welcome and encouraged. 


## ***"IPv6-only" is defined as the ability to function at full capacity with all features in the complete absense of legacy IPv4. For some entries, this may mean that they exist as dual stack but have 100% functionality from a client or peer that has no legacy IPv4.***

## This should probably turn into a database or better wiki page at some point. 


|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|**Software**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**Caveats and Notes**|
|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|Spotify|Desktop Client|Spotify|All|Y|N|Spotify desktop client does not work by default with in the absense of IPv4. Web and mobile applications work on IPv6-only. It is possible to run `command`|
|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|**Hardware**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**Caveats and Notes**|
|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|**Service**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**Caveats and Notes**|
|Github|Web|Microsoft|All|N|N|Some IPv6 support has been reported. GitHub.IO has v6 support but the main site does not.|
|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|**Processes**|**Platform**|**Vendor**|**Version**|**Supports IPv6**|**Suports IPv6 only**|**Caveats and Notes**|
|Apple recovery boot|MacOSX|Apple|All|U|N|System fails to pull recovery information upon restoration boot while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|Synology initial setup|DSM|Synology|All|U|N|DSM cannot discover setup host while connected to IPv6-only network with NAT64/DNS64. Works with dual stack|
|    |   |   |  |  |   |   |
|---|---|---|---|---|---|---|
|    |   |   |  |  |   |   |
|    |   |   |  |  |   |   |