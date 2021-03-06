---
title: WlanTimedConnectionRoaming rule (ndis)
description: The WlanTimedConnectionRoaming rule specifies that the NDIS miniport driver finishes the wireless LAN (WLAN) connection/roaming operations within 10 seconds.
ms.assetid: 0961C34B-FAD8-49ED-A0FD-5D790E973C4D
ms.author: windowsdriverdev
ms.date: 05/21/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
keywords: ["WlanTimedConnectionRoaming rule (ndis)"]
topic_type:
- apiref
api_name:
- WlanTimedConnectionRoaming
api_type:
- NA
---

# WlanTimedConnectionRoaming rule (ndis)


The **WlanTimedConnectionRoaming** rule specifies that the NDIS miniport driver finishes the wireless LAN (WLAN) connection/roaming operations within 10 seconds.

|              |      |
|--------------|------|
| Driver model | NDIS |

|                                   |                                                                                                                                        |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| Bug check(s) found with this rule | [**Bug Check 0xC4: DRIVER\_VERIFIER\_DETECTED\_VIOLATION**](https://msdn.microsoft.com/library/windows/hardware/ff560187) ( 0x00094008) |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At run time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Run [Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff545448) and select the [NDIS/WIFI verification](https://msdn.microsoft.com/library/windows/hardware/dn312128) option.</p></td>
</tr>
</tbody>
</table>

 

Applies to
----------

[**MiniportHaltEx**](https://msdn.microsoft.com/library/windows/hardware/ff559388)
[**MiniportOidRequest**](https://msdn.microsoft.com/library/windows/hardware/ff559416)
[**NdisMIndicateStatusEx**](https://msdn.microsoft.com/library/windows/hardware/ff563600)
See also
--------

[General Connection Operation Guidelines](https://msdn.microsoft.com/library/windows/hardware/ff552458)
 

 





