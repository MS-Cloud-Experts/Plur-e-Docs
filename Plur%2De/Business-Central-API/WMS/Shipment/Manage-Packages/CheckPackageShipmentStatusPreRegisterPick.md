**Request:**
```
{
  "ProcessMethod": "CheckPackageShipmentStatusPreRegisterPick",
  "Parameters": [
    {
      "WhsDocumentNo": "WHSE PICK-00035"
    }
  ]
}
```

**Output:** 

```
{
  "Response": "Waring: The Wshe Pick WHSE PICK-00035 that you are trying to register contains the following Unshipped Packages:\\\\Package No.: 1|2\\\\If you continue with the registration it will become partial and the unshipped packets will be deleted.\\\\Do you wish to continue?"
}
```

