**ProcessMethod**: GetPlureSetup

**Description**:
This method returns the Default Bin used to edit a Put-Away

**Parameters**: 

**Ouput**: Returns list of Bins available to be adjusted in the License Plate
-	**Bins**: is a Json array that contains the Bin Code and Location code to which each possible assignable BIN belongs.

**Example**:

```
**Request:**
{
  "ProcessMethod": "GetPlureSetup",
  "Parameters": []
}
```

![image.png](/.attachments/image-c171b508-367f-4b83-ac4a-8c032eddf7ee.png)

**Output:**
```
{
  "PlureSetup": {
    "id": 71017579,
    "name": "PLUSetup",
    "company": "CRONUS USA, Inc.",
    "position": "PLU Primary Key=CONST()",
    "recordId": "PLU Setup: \"\"",
    "primaryKey": {
      "fieldCount": 1,
      "fields": [
        {
          "id": 1,
          "name": "PLUPrimaryKey",
          "type": "Code",
          "value": null,
          "System": false
        }
      ]
    },
    "fieldCount": 45,
    "fields": [
      {
        "id": 1,
        "name": "PLUPrimaryKey",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 2,
        "name": "PLUEnabled",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 3,
        "name": "PLUNewSalesOrderProc",
        "type": "Integer",
        "value": null,
        "System": false
      },
      {
        "id": 4,
        "name": "PLUNewSOProcCap",
        "type": "Text",
        "value": null,
        "System": false
      },
      {
        "id": 5,
        "name": "PLUDefSalesLocation",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 6,
        "name": "PLUDefReturnsLocation",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 9,
        "name": "PLUId",
        "type": "GUID",
        "value": "{342E42D7-D8B8-457E-A21A-74472CE13E8E}",
        "System": false
      },
      {
        "id": 10,
        "name": "PLULastModifiedDate",
        "type": "DateTime",
        "value": "2022-11-22T17:07:27.2330000Z",
        "System": false
      },
      {
        "id": 11,
        "name": "PLUSalesOrderSeriesNo",
        "type": "Code",
        "value": "S-ORD",
        "System": false
      },
      {
        "id": 12,
        "name": "PLUSRetOrderSrsNo",
        "type": "Code",
        "value": "S-RETORD",
        "System": false
      },
      {
        "id": 13,
        "name": "PLUSalesMeasure",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 14,
        "name": "PLUEnableSalesInvoice",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 15,
        "name": "PLUEnableSalesOrder",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 16,
        "name": "PLUEnableReturnOrder",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 17,
        "name": "PLUSInvOrderSrsNo",
        "type": "Code",
        "value": "S-INV",
        "System": false
      },
      {
        "id": 18,
        "name": "PLUTextAPI",
        "type": "Text",
        "value": null,
        "System": false
      },
      {
        "id": 19,
        "name": "PLUJournalTemplateName",
        "type": "Code",
        "value": "PAYMENT",
        "System": false
      },
      {
        "id": 20,
        "name": "PLUJournalBatchName",
        "type": "Code",
        "value": "GENERAL",
        "System": false
      },
      {
        "id": 21,
        "name": "PLUSalesCrMemoSeriesNo",
        "type": "Code",
        "value": "S-CR",
        "System": false
      },
      {
        "id": 22,
        "name": "PLUEnableCrMemoOrder",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 23,
        "name": "PLUCompanyEnable",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 24,
        "name": "PLUWizardSetupCUID",
        "type": "Integer",
        "value": 71017585,
        "System": false
      },
      {
        "id": 25,
        "name": "PLUBalanceType",
        "type": "Option",
        "value": "Bank Account",
        "System": false
      },
      {
        "id": 26,
        "name": "PLUBalanceNo",
        "type": "Code",
        "value": "CHECKING",
        "System": false
      },
      {
        "id": 27,
        "name": "PLUArethereCustomers?",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 28,
        "name": "PLUArethereItems?",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 29,
        "name": "PLUArethereSalesPersons?",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 30,
        "name": "PLUPostedInvoiceNos",
        "type": "Code",
        "value": "S-INV+",
        "System": false
      },
      {
        "id": 31,
        "name": "PLUPostedCreditMemoNos",
        "type": "Code",
        "value": "S-CR+",
        "System": false
      },
      {
        "id": 32,
        "name": "PLUPostedPurchInvoice",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 33,
        "name": "PLUPostedPurchCreditM",
        "type": "Code",
        "value": null,
        "System": false
      },
      {
        "id": 34,
        "name": "PLUEnablePayments",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 35,
        "name": "PLUEnableSales",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 36,
        "name": "PLUEnableWMS",
        "type": "Boolean",
        "value": true,
        "System": false
      },
      {
        "id": 37,
        "name": "PLULicensePlateNos",
        "type": "Code",
        "value": "LP",
        "System": false
      },
      {
        "id": 38,
        "name": "PLUURLPlurE",
        "type": "Code",
        "value": "HTTPS://ADMINCENTER.PLUR-E.COM/",
        "System": false
      },
      {
        "id": 39,
        "name": "PLUInventoryCounting",
        "type": "Option",
        "value": "All",
        "System": false
      },
      {
        "id": 40,
        "name": "PLUDefaultLocation",
        "type": "Code",
        "value": "WMS",
        "System": false
      },
      {
        "id": 41,
        "name": "PLUDefaultBin",
        "type": "Code",
        "value": "FLOOR",
        "System": false
      },
      {
        "id": 42,
        "name": "PLUAutoGenerateSNLOT",
        "type": "Boolean",
        "value": false,
        "System": false
      },
      {
        "id": 2000000000,
        "name": "$systemId",
        "type": "GUID",
        "value": "{0E5864EB-6B6A-ED11-8C34-6045BDB8E0AA}",
        "System": false
      },
      {
        "id": 2000000001,
        "name": "SystemCreatedAt",
        "type": "DateTime",
        "value": "2022-11-22T13:45:31.4570000Z",
        "System": false
      },
      {
        "id": 2000000002,
        "name": "SystemCreatedBy",
        "type": "GUID",
        "value": "{00000000-0000-0000-0000-000000000001}",
        "System": false
      },
      {
        "id": 2000000003,
        "name": "SystemModifiedAt",
        "type": "DateTime",
        "value": "2022-12-15T13:25:26.5830000Z",
        "System": false
      },
      {
        "id": 2000000004,
        "name": "SystemModifiedBy",
        "type": "GUID",
        "value": "{D6194FDA-68F1-4DEA-9340-75AF3121F16F}",
        "System": false
      }
    ]
  }
}
```
