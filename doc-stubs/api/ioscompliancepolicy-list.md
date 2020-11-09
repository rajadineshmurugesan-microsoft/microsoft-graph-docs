---
title: "List iosCompliancePolicies"
description: "Get a list of the iosCompliancePolicy objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List iosCompliancePolicies
Namespace: microsoft.graph

Get a list of the [iosCompliancePolicy](../resources/ioscompliancepolicy.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

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
GET ** Collection URI for microsoft.graph.iosCompliancePolicy not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/ioscompliancepolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ioscompliancepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.iosCompliancePolicy not found
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.iosCompliancePolicy)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "86f00a52-0a52-86f0-520a-f086520af086",
      "roleScopeTagIds": [
        "String"
      ],
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "displayName": "String",
      "version": "Integer",
      "passcodeBlockSimple": "Boolean",
      "passcodeExpirationDays": "Integer",
      "passcodeMinimumLength": "Integer",
      "passcodeMinutesOfInactivityBeforeLock": "Integer",
      "passcodeMinutesOfInactivityBeforeScreenTimeout": "Integer",
      "passcodePreviousPasscodeBlockCount": "Integer",
      "passcodeMinimumCharacterSetCount": "Integer",
      "passcodeRequiredType": "String",
      "passcodeRequired": "Boolean",
      "osMinimumVersion": "String",
      "osMaximumVersion": "String",
      "osMinimumBuildVersion": "String",
      "osMaximumBuildVersion": "String",
      "securityBlockJailbrokenDevices": "Boolean",
      "deviceThreatProtectionEnabled": "Boolean",
      "deviceThreatProtectionRequiredSecurityLevel": "String",
      "advancedThreatProtectionRequiredSecurityLevel": "String",
      "managedEmailProfileRequired": "Boolean",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem"
        }
      ]
    }
  ]
}
```
