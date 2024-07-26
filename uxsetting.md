---
title: "uxSetting resource type"
description: "UXSetting resource Type"
author: "skashyap7"
ms.localizationpriority: medium
ms.subservice: "entra-directory-management"
doc_type: resourcePageType
---

# uxSetting resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents settings relating to access to the Microsoft Entra admin center. 

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get](../api/uxsetting-get.md)|[uxSetting](../resources/uxsetting.md)|Read the properties and relationships of a [uxSetting](../resources/uxsetting.md) object.|
|[Update](../api/uxsetting-update.md)|[uxSetting](../resources/uxsetting.md)|Update the properties of a [uxSetting](../resources/uxsetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|restrictNonAdminAccess|nonAdminSetting|If set to `true`, nonadministrators can't browse the Microsoft Entra admin center. Nonadministrators  who are owners of groups or applications are unable to use the Azure portal to manage their owned resources. If set to `false`, nonadministrators can browse the Microsoft Entra admin center. The possible values are: `true`, `false`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource type.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.uxSetting",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.uxSetting",
  "restrictNonAdminAccess": "String"
}
```

