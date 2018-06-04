---
Description: The CheckTransform method checks whether an input media type is compatible with an output media type. This method overrides the CTransformFilter::CheckTransform method.
ms.assetid: d0953014-4a49-4738-a449-c247396a6794
title: CTransInPlaceFilter.CheckTransform method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CTransInPlaceFilter.CheckTransform method

The `CheckTransform` method checks whether an input media type is compatible with an output media type. This method overrides the [**CTransformFilter::CheckTransform**](ctransformfilter-checktransform.md) method.

## Syntax


```C++
HRESULT CheckTransform(
   const CMediaType *mtIn,
   const CMediaType *mtOut
);
```



## Parameters

<dl> <dt>

*mtIn* 
</dt> <dd>

Pointer to a [**CMediaType**](cmediatype.md) object that specifies the input type.

</dd> <dt>

*mtOut* 
</dt> <dd>

Pointer to a **CMediaType** object that specifies the output type.

</dd> </dl>

## Return value

Returns S\_OK.

## Remarks

The **CTransInPlace** filter never calls `CheckTransform`. Instead, all pin connection use [**CTransformFilter::CheckInputType**](ctransformfilter-checkinputtype.md) to check the media type, with the assumption that the input and output types always match.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Transip.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CTransInPlaceFilter Class**](ctransinplacefilter.md)
</dt> </dl>

 

 



