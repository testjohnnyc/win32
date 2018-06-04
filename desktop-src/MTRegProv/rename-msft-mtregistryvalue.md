---
title: Rename method of the MSFT\_MTRegistryValue class
description: Renames the registry value object.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: d8cd16db-799a-45dd-b08b-8e0a86afccf4
ms.prod: windows-server-dev
ms.technology: windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- Rename method
- Rename method, MSFT_MTRegistryValue class
- MSFT_MTRegistryValue class, Rename method
topic_type:
- apiref
api_name:
- MSFT_MTRegistryValue.Rename
api_location:
- RegProv.dll
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Rename method of the MSFT\_MTRegistryValue class

Renames the registry value object.

## Syntax


```mof
uint32 Rename(
  [in]  string               NewName,
  [out] MSFT_MTRegistryValue Result
);
```



## Parameters

<dl> <dt>

*NewName* \[in\]
</dt> <dd>

The fully qualified new name of the object.

</dd> <dt>

*Result* \[out\]
</dt> <dd>

On success, returns an [**MSFT\_MTRegistryValue**](msft-mtregistryvalue.md) embedded instance containing the new object with the new path.

</dd> </dl>

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                              |
| Minimum supported server<br/> | Windows Server 2016<br/>                                                         |
| Namespace<br/>                | Root\\Microsoft\\Windows\\ManagementTools<br/>                                   |
| MOF<br/>                      | <dl> <dt>RegProv.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RegProv.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_MTRegistryValue**](msft-mtregistryvalue.md)
</dt> </dl>

 

 




