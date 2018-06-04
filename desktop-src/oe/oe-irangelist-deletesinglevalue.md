---
title: IRangeList DeleteSingleValue method
description: Removes a single value to the message range list.
ms.assetid: 8726fdff-5c0f-4ea6-9657-38ff7406bf0a
keywords:
- DeleteSingleValue method Windows Mail (formerly Outlook Express)
- DeleteSingleValue method Windows Mail (formerly Outlook Express) , IRangeList interface
- IRangeList interface Windows Mail (formerly Outlook Express) , DeleteSingleValue method
topic_type:
- apiref
api_name:
- IRangeList.DeleteSingleValue
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

# IRangeList::DeleteSingleValue method

\[**IRangeList::DeleteSingleValue** is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.\]

Removes a single value to the message range list.

## Syntax


```C++
HRESULT DeleteSingleValue(
  [in] const ULONG value
);
```



## Parameters

<dl> <dt>

*value* \[in\]
</dt> <dd>

Type: **const ULONG**

Specifies the single value to delete from the range list.



| Value                                                                                                                                                                                                                                 | Meaning                                               |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| <span id="RL_LAST_MESSAGE"></span><span id="rl_last_message"></span><dl> <dt>**RL\_LAST\_MESSAGE**</dt> <dt>((ULONG)-1)</dt> </dl> | Equivalent to "\*" in an IMAP range list. <br/> |



 

</dd> </dl>

## Return value

Type: **HRESULT**

Returns one of the following values.



| Return code                                                                                   | Description                                                     |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Indicates success.<br/>                                   |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Indicates that an attempt to allocate memory failed.<br/> |



 

## Remarks

For example, **DeleteSingleValue**(42) removes 42 from the range list.

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                                                    |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                           |
| Product<br/>                  | Outlook Express 6.0<br/>                                                                                 |
| Header<br/>                   | <dl> <dt>Imnxport.h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Imnxport.idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Inetcomm.dll (version 6.0 or later)</dt> </dl> |



 

 




