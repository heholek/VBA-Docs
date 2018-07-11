---
title: Pages.BeforePageDelete Event (Visio)
keywords: vis_sdr.chm11019050
f1_keywords:
- vis_sdr.chm11019050
ms.prod: visio
api_name:
- Visio.Pages.BeforePageDelete
ms.assetid: 52fbea6b-0258-8610-74e2-74ade9f8ae49
ms.date: 06/08/2017
---


# Pages.BeforePageDelete Event (Visio)

Occurs before a page is deleted.


## Syntax

Private Sub  _expression_ _'BeforePageDelete'(**_ByVal Page As [IVPAGE]_**)

 _expression_ A variable that represents a [Pages](./Visio.Pages.md) object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Page_|Required| **[IVPAGE]**|The page that is going to be deleted.|

## Remarks

If you're using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own  **Event** objects, use the **Add** or **AddAdvise** method. To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. To create an **Event** object that receives notification, use the **AddAdvise** method. To find an event code for the event you want to create, see[Event codes](../visio/Concepts/event-codesvisio.md).

