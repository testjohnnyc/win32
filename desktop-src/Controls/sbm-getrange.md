---
title: SBM\_GETRANGE message
description: The SBM\_GETRANGE message is sent to retrieve the minimum and maximum position values for the scroll bar control.
ms.assetid: '661a9491-3bf6-4685-aea0-c5e4126313af'
keywords: ["SBM_GETRANGE message Windows Controls"]
topic_type:
- apiref
api_name:
- SBM_GETRANGE
api_location:
- Winuser.h
api_type:
- HeaderDef
---

# SBM\_GETRANGE message

The **SBM\_GETRANGE** message is sent to retrieve the minimum and maximum position values for the scroll bar control.

Applications should not send this message directly. Instead, they should use the [**GetScrollRange**](getscrollrange.md) function. A window receives this message through its [*WindowProc*](https://msdn.microsoft.com/library/windows/desktop/ms633573) function. Applications which implement a custom scroll bar control must respond to these messages for the **GetScrollRange** function to work properly.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Pointer to a variable that receives the minimum scrolling position.

</dd> <dt>

*lParam* 
</dt> <dd>

Pointer to a variable that receives the maximum scrolling position.

</dd> </dl>

## Return value

This message does not return a value.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

**Reference**
</dt> <dt>

[**SBM\_GETPOS**](sbm-getpos.md)
</dt> <dt>

[**SBM\_SETPOS**](sbm-setpos.md)
</dt> <dt>

[**SBM\_SETRANGE**](sbm-setrange.md)
</dt> <dt>

[**SBM\_SETRANGEREDRAW**](sbm-setrangeredraw.md)
</dt> </dl>

�

�




