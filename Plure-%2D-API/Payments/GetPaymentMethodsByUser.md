**HttpMethod:**
```
GET
```

**Endpoint:**
```
 {{apiurl}}/api/{{apiversion}}/payments/GetPaymentMethodsByUser?customerId={{customerId}}&environmentId={{environmentId}}&mobileUserId={{mobileUserId}}
```

**Parameters:**
| No. | Parameter | Type | Value |
|--|--|--|--|
|1|apiurl|string|https://api.plur-e.com/|
|2|apiversion|string|v1.0|
|3|customerId|string|Subscription customer Id|
|4|environmentId|string|Environment Id |
|5|mobileUserId|string||



**Headers:**
```
PlureApiKey: pk_QjJ4Wj7LRKCrdZ6CTPVDEGc63AbVwUxHrMgeJkQcM5f39T7rTkw9U3pWpjMkUVKNPqBFAATNwfYRqnVNpFy8Xm7qSZAWGDnETyL7
```

**Authentication:**
```
Bearer token: {{authentication}}
```

**Payload:**
```
```

**Result ex:**
```
[
    {
        "paymentMethodId": "pm_c8429cfe53874768bf0b8f0f52f47a61",
        "customerId": "cus_MqePl07DKnPzxD",
        "name": "Cash",
        "paymentType": 1,
        "environmentId": "env_e4e29085f189483cb37dfdf6bf514165",
        "environment": {
            "environmentId": "env_e4e29085f189483cb37dfdf6bf514165",
            "customerId": "cus_MqePl07DKnPzxD",
            "platformCode": "D365BC",
            "description": "NoBorrar",
            "environmentType": 1
        },
        "journalBatchName": "CASH",
        "createdOn": "2023-06-28T13:56:26.3258348-05:00",
        "createdById": "usr_57e2ad681ca14a38a83ed07b381d7900",
        "createdBy": {
            "userId": "usr_57e2ad681ca14a38a83ed07b381d7900",
            "name": "Raul Ocampo"
        },
        "modifiedOn": "2023-06-28T13:56:26.325953-05:00",
        "modifiedById": "usr_57e2ad681ca14a38a83ed07b381d7900",
        "modifiedBy": {
            "userId": "usr_57e2ad681ca14a38a83ed07b381d7900",
            "name": "Raul Ocampo"
        }
    },
    {
        "paymentMethodId": "pm_104ba5e16b364749b9db05d3f7271d43",
        "customerId": "cus_MqePl07DKnPzxD",
        "name": "Card",
        "paymentType": 2,
        "environmentId": "env_e4e29085f189483cb37dfdf6bf514165",
        "environment": {
            "environmentId": "env_e4e29085f189483cb37dfdf6bf514165",
            "customerId": "cus_MqePl07DKnPzxD",
            "platformCode": "D365BC",
            "description": "NoBorrar",
            "environmentType": 1
        },
        "journalBatchName": "GENERAL",
        "createdOn": "2023-06-28T15:36:33.1908189-05:00",
        "createdById": "usr_57e2ad681ca14a38a83ed07b381d7900",
        "createdBy": {
            "userId": "usr_57e2ad681ca14a38a83ed07b381d7900",
            "name": "Raul Ocampo"
        },
        "modifiedOn": "2023-06-28T15:36:33.1909025-05:00",
        "modifiedById": "usr_57e2ad681ca14a38a83ed07b381d7900",
        "modifiedBy": {
            "userId": "usr_57e2ad681ca14a38a83ed07b381d7900",
            "name": "Raul Ocampo"
        }
    }
]
```
