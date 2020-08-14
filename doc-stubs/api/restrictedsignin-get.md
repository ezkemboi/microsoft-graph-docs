---
title: "Get restrictedSignIn"
description: "Read the properties and relationships of a restrictedSignIn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get restrictedSignIn
Namespace: microsoft.graph

Read the properties and relationships of a [restrictedSignIn](../resources/restrictedsignin.md) object.

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
GET /auditLogs/restrictedSignIns/{restrictedSignInId}
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

If successful, this method returns a `200 OK` response code and a [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/restrictedSignIns/{restrictedSignInId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedSignIn"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedSignIn",
    "id": "0aa782bf-82bf-0aa7-bf82-a70abf82a70a",
    "alternateSignInName": "String",
    "appDisplayName": "String",
    "appId": "String",
    "appliedConditionalAccessPolicies": [
      {
        "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
      }
    ],
    "authenticationDetails": [
      {
        "@odata.type": "microsoft.graph.authenticationDetail"
      }
    ],
    "authenticationMethodsUsed": [
      "String"
    ],
    "authenticationProcessingDetails": [
      {
        "@odata.type": "microsoft.graph.keyValue"
      }
    ],
    "authenticationRequirement": "String",
    "authenticationRequirementPolicies": [
      {
        "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
      }
    ],
    "clientAppUsed": "String",
    "conditionalAccessStatus": "String",
    "correlationId": "String",
    "createdDateTime": "String (timestamp)",
    "deviceDetail": {
      "@odata.type": "microsoft.graph.deviceDetail"
    },
    "isInteractive": "Boolean",
    "ipAddress": "String",
    "location": {
      "@odata.type": "microsoft.graph.signInLocation"
    },
    "mfaDetail": {
      "@odata.type": "microsoft.graph.mfaDetail"
    },
    "networkLocationDetails": [
      {
        "@odata.type": "microsoft.graph.networkLocationDetail"
      }
    ],
    "originalRequestId": "String",
    "processingTimeInMilliseconds": "Integer",
    "riskDetail": "String",
    "riskEventTypes": [
      "String"
    ],
    "riskEventTypes_v2": [
      "String"
    ],
    "riskLevelAggregated": "String",
    "riskLevelDuringSignIn": "String",
    "riskState": "String",
    "resourceDisplayName": "String",
    "resourceId": "String",
    "resourceTenantId": "String",
    "servicePrincipalId": "String",
    "servicePrincipalName": "String",
    "signInEventTypes": [
      "String"
    ],
    "status": {
      "@odata.type": "microsoft.graph.signInStatus"
    },
    "tokenIssuerName": "String",
    "tokenIssuerType": "String",
    "userAgent": "String",
    "userDisplayName": "String",
    "userId": "String",
    "userPrincipalName": "String",
    "targetTenantId": "Guid"
  }
}
```
