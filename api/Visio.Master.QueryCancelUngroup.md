---
title: Master.QueryCancelUngroup Event (Visio)
keywords: vis_sdr.chm10719330
f1_keywords:
- vis_sdr.chm10719330
ms.prod: visio
api_name:
- Visio.Master.QueryCancelUngroup
ms.assetid: 44ce0f2e-e877-ec7f-b5ec-1c3ff3b9749a
ms.date: 06/08/2017
---


# Master.QueryCancelUngroup Event (Visio)

Occurs before the application ungroups a selection of shapes in response to a user action in the interface. If any event handler returns  **True** , the operation is canceled.


## Syntax

Private Sub  _expression_ _'QueryCancelUngroup'(**_ByVal Selection As [IVSELECTION]_**)

 _expression_ A variable that represents a [Master](./Visio.Master.md) object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Selection_|Required| **[IVSELECTION]**|The selection of shapes that is going to be ungrouped.|

## Remarks

A Microsoft Visio instance fires  **QueryCancelUngroup** after the user has directed the instance to ungroup one or more shapes.




- If any event handler returns  **True** (cancel), the instance fires **UngroupCanceled** and does not ungroup the shapes.
    
- If all handlers return  **False** (don't cancel), the instance fires **ShapeParentChanged** , **BeforeSelectionDelete** , and **BeforeShapeDelete** , and then ungroups the shapes.
    


While a Visio instance is firing a query or cancel event, it respondsto inquiries from client code but refuses to perform operations. Client code can show forms or message boxes while responding to a query or cancel event.

If you're using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own  **Event** objects, use the **Add** or **AddAdvise** method. To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. To create an **Event** object that receives notification, use the **AddAdvise** method. To find an event code for the event you want to create, see[Event codes](../visio/Concepts/event-codesvisio.md).

