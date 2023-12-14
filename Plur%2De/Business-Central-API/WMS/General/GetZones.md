**Request:**
```
{
  "ProcessMethod": "GetZones",
  "Parameters": [
    {
      "LocationCode": "Asia"
    }
  ]
}
```

**Ouput:**


```
{
  "Zones": [
    {
      "Code": "PICK",
      "LocationCode": "ASIA",
      "Description": "Picking",
      "BinTypeCode": "PICK",
      "LocationArray": [
        {
          "Code": "ASIA",
          "Name": "ASIA - CABRINHA WAREHOUSE",
          "DefaultBinCode": "",
          "RequirePutaway": true,
          "RequirePick": true,
          "RequireReceive": true,
          "RequireShipment": true,
          "BinMandatory": true,
          "DirectedPutawayandPick": true,
          "BinArray": [
            {
              "Code": "AJUST",
              "Description": "Ajustment",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "PICK",
              "Description": "Picking",
              "ZoneCode": "PICK",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC1",
              "Description": "Receiving 1",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC2",
              "Description": "Receiving 2",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "SHIP",
              "Description": "Shipping",
              "ZoneCode": "SHIP",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO1",
              "Description": "Storage 1",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO2",
              "Description": "Storage 2",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            }
          ]
        }
      ]
    },
    {
      "Code": "REC",
      "LocationCode": "ASIA",
      "Description": "Receiving",
      "BinTypeCode": "RECEIVE",
      "LocationArray": [
        {
          "Code": "ASIA",
          "Name": "ASIA - CABRINHA WAREHOUSE",
          "DefaultBinCode": "",
          "RequirePutaway": true,
          "RequirePick": true,
          "RequireReceive": true,
          "RequireShipment": true,
          "BinMandatory": true,
          "DirectedPutawayandPick": true,
          "BinArray": [
            {
              "Code": "AJUST",
              "Description": "Ajustment",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "PICK",
              "Description": "Picking",
              "ZoneCode": "PICK",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC1",
              "Description": "Receiving 1",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC2",
              "Description": "Receiving 2",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "SHIP",
              "Description": "Shipping",
              "ZoneCode": "SHIP",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO1",
              "Description": "Storage 1",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO2",
              "Description": "Storage 2",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            }
          ]
        }
      ]
    },
    {
      "Code": "SHIP",
      "LocationCode": "ASIA",
      "Description": "Shipping",
      "BinTypeCode": "SHIP",
      "LocationArray": [
        {
          "Code": "ASIA",
          "Name": "ASIA - CABRINHA WAREHOUSE",
          "DefaultBinCode": "",
          "RequirePutaway": true,
          "RequirePick": true,
          "RequireReceive": true,
          "RequireShipment": true,
          "BinMandatory": true,
          "DirectedPutawayandPick": true,
          "BinArray": [
            {
              "Code": "AJUST",
              "Description": "Ajustment",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "PICK",
              "Description": "Picking",
              "ZoneCode": "PICK",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC1",
              "Description": "Receiving 1",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC2",
              "Description": "Receiving 2",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "SHIP",
              "Description": "Shipping",
              "ZoneCode": "SHIP",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO1",
              "Description": "Storage 1",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO2",
              "Description": "Storage 2",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            }
          ]
        }
      ]
    },
    {
      "Code": "STO",
      "LocationCode": "ASIA",
      "Description": "Storage",
      "BinTypeCode": "STO",
      "LocationArray": [
        {
          "Code": "ASIA",
          "Name": "ASIA - CABRINHA WAREHOUSE",
          "DefaultBinCode": "",
          "RequirePutaway": true,
          "RequirePick": true,
          "RequireReceive": true,
          "RequireShipment": true,
          "BinMandatory": true,
          "DirectedPutawayandPick": true,
          "BinArray": [
            {
              "Code": "AJUST",
              "Description": "Ajustment",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "PICK",
              "Description": "Picking",
              "ZoneCode": "PICK",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC1",
              "Description": "Receiving 1",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "REC2",
              "Description": "Receiving 2",
              "ZoneCode": "REC",
              "LocationCode": "ASIA"
            },
            {
              "Code": "SHIP",
              "Description": "Shipping",
              "ZoneCode": "SHIP",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO1",
              "Description": "Storage 1",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            },
            {
              "Code": "STO2",
              "Description": "Storage 2",
              "ZoneCode": "STO",
              "LocationCode": "ASIA"
            }
          ]
        }
      ]
    }
  ]
}
```
