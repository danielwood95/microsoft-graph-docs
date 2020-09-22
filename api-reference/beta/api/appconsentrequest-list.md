---
title: "List appConsentRequests"
description: "Get a list of the appConsentRequest objects and their properties."
author: "davidmu1"
localization_priority: Normal
ms.prod: "microsoft-identity-platform"
doc_type: apiPageType
---

# List appConsentRequests

Namespace: microsoft.graph

Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type | Permissions (from most to least privileged) |
|:---|:---|
| Delegated (work or school account) | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## Optional query parameters

This method supports the `$filter`, `$select`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name | Description |
|:---|:---|
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appConsentRequests",
  "value": [
    {
      "odata.type": "#microsoft.graph.appConsentRequest",
      "id": "5a3a0f94-b89d-4cd3-a4ad-fd78faec333f",
      "appId": "3fa97b03-0af0-4773-93ed-4c247cb62ce2",
      "appDisplayName": "Salesforce",
      "consentType": "Dynamic",
      "pendingScopes": [
        {
          "displayName": "Salesforce.ReadWrite.Users"
        },
        {
          "displayName": "Salesforce.ReadWrite.Groups"
        }
      ]    
    }
  ]
}
```