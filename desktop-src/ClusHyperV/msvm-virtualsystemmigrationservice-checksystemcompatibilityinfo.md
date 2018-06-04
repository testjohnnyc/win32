---
title: CheckSystemCompatibilityInfo method of the Msvm\_VirtualSystemMigrationService class
description: Verifies whether a computer system is able to host the specified virtual machine (VM).
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 125db9ca-b171-46f0-95e6-19008d2a9652
ms.prod: windows-server-dev
ms.technology:
- failover-cluster-hyperv
- windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- CheckSystemCompatibilityInfo method
- CheckSystemCompatibilityInfo method, Msvm_VirtualSystemMigrationService class
- Msvm_VirtualSystemMigrationService class, CheckSystemCompatibilityInfo method
topic_type:
- apiref
api_name:
- Msvm_VirtualSystemMigrationService.CheckSystemCompatibilityInfo
api_location:
- VMMS.exe
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CheckSystemCompatibilityInfo method of the Msvm\_VirtualSystemMigrationService class

Verifies whether a computer system is able to host the specified virtual machine (VM).

This method uses compatibility information that is generated by the [**GetSystemCompatibilityInfo**](msvm-virtualsystemmigrationservice-getsystemcompatibilityinfo.md) method.

## Syntax


```mof
uint32 CheckSystemCompatibilityInfo(
  [in]  uint8  CompatibilityInfo[],
  [out] string Reasons[]
);
```



## Parameters

<dl> <dt>

*CompatibilityInfo* \[in\]
</dt> <dd>

An opaque blob generated by the [**GetSystemCompatibilityInfo**](msvm-virtualsystemmigrationservice-getsystemcompatibilityinfo.md) method that represents either one VM or all VMs hosted by a computer system.

</dd> <dt>

*Reasons* \[out\]
</dt> <dd>

An array of strings containing [**Msvm\_Error**](msvm-error.md) instances in CIM-XML format representing warnings or error information. These strings can be passed to the [**FormatError**](msvm-virtualsystemmanagementservice-formaterror.md) method to generate error messages.

</dd> </dl>

## Return value

The possible return values are:

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Method Parameters Checked - Job Started** (4096)
</dt> <dt>

**Failed** (32768)
</dt> <dt>

**Access Denied** (32769)
</dt> <dt>

**Not Supported** (32770)
</dt> <dt>

**Status is unknown** (32771)
</dt> <dt>

**Timeout** (32772)
</dt> <dt>

**Invalid parameter** (32773)
</dt> <dt>

**System is in use** (32774)
</dt> <dt>

**Invalid state for this operation** (32775)
</dt> <dt>

**Incorrect data type** (32776)
</dt> <dt>

**System is not available** (32777)
</dt> <dt>

**Out of memory** (32778)
</dt> <dt>

**Not compatible** (32784)
</dt> </dl>

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                              |
| Minimum supported server<br/> | Windows Server 2016<br/>                                                                         |
| Namespace<br/>                | Root\\HyperVCluster\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsHyperVCluster.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>VMMS.exe</dt> </dl>                    |



## See also

<dl> <dt>

[**Msvm\_VirtualSystemMigrationService**](msvm-virtualsystemmigrationservice.md)
</dt> </dl>

 

 




