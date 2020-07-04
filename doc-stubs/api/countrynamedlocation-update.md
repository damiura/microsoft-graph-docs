---
title: "Update countryNamedLocation"
description: "Update the properties of a countryNamedLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update countryNamedLocation
Namespace: microsoft.graph

Update the properties of a [countryNamedLocation](../resources/countrynamedlocation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /countryNamedLocation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [countryNamedLocation](../resources/countrynamedlocation.md) object.

The following table shows the properties that are required when you create the [countryNamedLocation](../resources/countrynamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|countriesAndRegions|String collection|**TODO: Add Description**|
|includeUnknownCountriesAndRegions|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/countryNamedLocation
Content-Type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "displayName": "String",
  "countriesAndRegions": [
    "String"
  ],
  "includeUnknownCountriesAndRegions": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "id": "0b39b27a-b27a-0b39-7ab2-390b7ab2390b",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "countriesAndRegions": [
    "String"
  ],
  "includeUnknownCountriesAndRegions": "Boolean"
}
```
