---
Description: Represents a single extended key usage (EKU) property of a certificate.
ms.assetid: 78f9f9cb-46e7-4f81-a16e-503750a0d743
title: EKU object
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: interface
ms.date: 05/31/2018
---

# EKU object

\[CAPICOM is a 32-bit only component that is available for use in the following operating systems: Windows Server 2008, Windows Vista, and Windows XP. Instead, use the [**X509EnhancedKeyUsageExtension Class**](https://www.bing.com/search?q=**X509EnhancedKeyUsageExtension Class**) in the [**System.Security.Cryptography.X509Certificates**](https://www.bing.com/search?q=**System.Security.Cryptography.X509Certificates**) namespace.\]

The **EKU** object represents a single extended key usage (EKU) property of a certificate.

## Members

The **EKU** object has these types of members:

-   [Properties](#properties)

### Properties

The **EKU** object has these properties.



| Property                            | Access type           | Description                                                                                                                                                                                                   |
|:------------------------------------|:----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Name**](eku-name.md)<br/> | Read/write<br/> | Sets or retrieves an enumeration value that specifies the CAPICOM name of the EKU. This is the default property.<br/>                                                                                   |
| [**OID**](eku-oid.md)<br/>   | Read/write<br/> | Sets or retrieves a string that contains an EKU [*object identifier*](https://www.bing.com/search?q=*object identifier*) (OID) string value as defined in Wincrypt.h.<br/> |



 

## Remarks

The **EKU** object is used by the following collection and property:

-   [**EKUs**](ekus.md) collection
-   [**CertificateStatus.EKU**](certificatestatus-eku.md) property

The **EKU** object cannot be created.

## Requirements



|                                  |                                                                                        |
|----------------------------------|----------------------------------------------------------------------------------------|
| End of client support<br/> | Windows Vista<br/>                                                               |
| End of server support<br/> | Windows Server 2008<br/>                                                         |
| Redistributable<br/>       | CAPICOM 2.0 or later on Windows Server 2003 and Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



 

 



