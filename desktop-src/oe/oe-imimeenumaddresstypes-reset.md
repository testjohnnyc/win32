---
title: IMimeEnumAddressTypes Reset method
description: Resets the enumeration sequence to the beginning.
ms.assetid: d8942289-f706-4433-b2d6-f3db71ff5d4c
keywords:
- Reset method Windows Mail (formerly Outlook Express)
- Reset method Windows Mail (formerly Outlook Express) , IMimeEnumAddressTypes interface
- IMimeEnumAddressTypes interface Windows Mail (formerly Outlook Express) , Reset method
topic_type:
- apiref
api_name:
- IMimeEnumAddressTypes.Reset
api_location:
- Inetcomm.dll
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IMimeEnumAddressTypes::Reset method

Resets the enumeration sequence to the beginning.

## Syntax


```C++
HRESULT Reset();
```



## Parameters

This method has no parameters.

## Return value

Type: **HRESULT**

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                                                    |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                           |
| Product<br/>                  | Outlook Express 6.0<br/>                                                                                 |
| Header<br/>                   | <dl> <dt>Mimeole.h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Mimeole.idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Inetcomm.dll (version 6.0 or later)</dt> </dl> |



 

 




