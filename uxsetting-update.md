---
title: "Update uxSetting"
description: "Update the properties of a uxSetting object."
author: "skashyap7"
ms.localizationpriority: medium
ms.subservice: "entra-directory-management"
doc_type: apiPageType
---

# Update uxSetting
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [uxSetting](../resources/uxsetting.md) object.

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/entra/uxSetting
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|restrictNonAdminAccess|nonAdminSetting|If set to `true`, nonadministrators can't browse the Microsoft Entra admin center. Nonadministrators  who are owners of groups or applications are unable to use the Azure portal to manage their owned resources. If set to `false`, nonadministrators can browse the Microsoft Entra admin center. The possible values are: `true`, `false`.|



## Response

If successful, this method returns a `204 No Content` response code. It doesn't return anything in the response body.

## Examples

### Request
The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "update_uxsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/entra/uxSetting
Content-Type: application/json

{
  "restrictNonAdminAccess": "true",
  "tenantId" : "00000000-0000-0000-0000-000000000000"
}
```


### Response
The following example shows the response

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


