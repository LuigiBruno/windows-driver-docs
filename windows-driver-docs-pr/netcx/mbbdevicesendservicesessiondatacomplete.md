---
title: MbbDeviceSendServiceSessionDataComplete
description: The MbbDeviceSendServiceSessionDataComplete method frees memory previously allocated by MBBCx for device service session data sent to the device.
ms.assetid: 83004F03-95AC-4B70-AE9B-1DA1956281C5
keywords:
- Mobile Broadband WDF Class Extension MbbDeviceSendServiceSessionDataComplete, MBBCx MbbDeviceSendServiceSessionDataComplete
ms.author: windowsdriverdev
ms.date: 03/21/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# MbbDeviceSendServiceSessionDataComplete

[!include[MBBCx Beta Prerelease](../mbbcx-beta-prerelease.md)]

The **MbbDeviceSendServiceSessionDataComplete** method frees memory previously allocated by MBBCx for device service session data sent to the device.

## Syntax

```C++
VOID
MbbDeviceSendServiceSessionDataComplete(
    _In_ WDFMEMORY Data,
    _In_ NTSTATUS NtStatus
);
```

## Parameters

*Data* [in]  
A WDFMEMORY object that contains data passed to the device.

*NtStatus* [in]  
An NTSTATUS value indicating the status of the send operation.

## Return value

This method does not return a value.

## Remarks

Client drivers must call this method from within the [*EvtMbbDeviceSendServiceSessionData*](evt-mbb-device-send-service-session-data.md) callback function after they have sent the DSS data to the device.

## Requirements

|     |     |
| --- | --- |
| Target platform | Universal |
| Minimum KMDF version | 1.27 |
| Header | Mbbcx.h |
| IRQL | PASSIVE_LEVEL |