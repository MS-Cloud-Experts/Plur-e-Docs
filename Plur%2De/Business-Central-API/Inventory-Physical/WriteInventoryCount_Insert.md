### API Documentation: WriteInventoryCount_Insert

#### **Overview**
The `WriteInventoryCount_Insert` API allows the insertion of inventory count entries into the item journal. It processes multiple item journal lines, including serial numbers if applicable, and records these counts into the physical inventory journal. Additionally, it calculates any discrepancies between physical counts and system-calculated quantities, ensuring the appropriate updates are made to Business Central's inventory.

#### **Request Structure**
```json
{
  "ProcessMethod": "WriteInventoryCount_Insert",
  "Parameters": [
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "PostingDate": "2024-06-13",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "T0MLXXX",
      "Description": "",
      "LocationCode": "ASIA TEMP",
      "SalespersPurchCode": "",
      "QtyPhysInventory": 1322,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "SerialJA": [
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X14q"
        },
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X15q"
        }
      ]
    },
    {
      "JournalTemplateName": "PHYS. INV.",
      "JournalBatchName": "DEFAULT",
      "PostingDate": "2024-06-13",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "T0SMXXX",
      "Description": "",
      "LocationCode": "ASIA TEMP",
      "SalespersPurchCode": "",
      "QtyPhysInventory": 30,
      "UserID": "",
      "TimeStampMovil": "2024-06-13T00:00:00",
      "SerialJA": [
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X14"
        },
        {
          "LineNo": 20000,
          "ItemNo": "SERIAL2",
          "VariantCode": "",
          "LotNo": "",
          "SerialNo": "X15"
        }
      ]
    }
  ]
}
```

#### **Parameters**
- **ProcessMethod**: Indicates the method to invoke, in this case `"WriteInventoryCount_Insert"`.
- **Parameters**: An array of objects describing the inventory journal lines.
  - **JournalTemplateName**: The name of the journal template being used (e.g., `"PHYS. INV."`).
  - **JournalBatchName**: The name of the journal batch (e.g., `"DEFAULT"`).
  - **PostingDate**: The posting date of the journal entry (e.g., `"2024-06-13"`).
  - **DocumentNo**: The document number for this entry (e.g., `"SSDS"`).
  - **ItemNo**: The item number being processed (e.g., `"SERIAL2"`).
  - **VariantCode**: The variant code of the item, if applicable (e.g., `"T0MLXXX"`).
  - **Description**: A description of the item.
  - **LocationCode**: The location code where the item is stored (e.g., `"ASIA TEMP"`).
  - **SalespersPurchCode**: The salesperson or purchaser code, if applicable.
  - **QtyPhysInventory**: The physical inventory quantity counted (e.g., `1322`).
  - **UserID**: The user ID that processed this entry.
  - **TimeStampMovil**: A timestamp for mobile processing (e.g., `"2024-06-13T00:00:00"`).
  - **SerialJA**: An array of serial numbers if the item is serialized.

#### **Example Response**
```json
{
  "WriteInventoryCount_Insert": [
    {
      "JournalTemplateName": "PHYS. INVE",
      "JournalBatchName": "DEFAULT",
      "PostingDate": "2024-06-13",
      "EntryType": "Positive Adjmt.",
      "DocumentNo": "SSDS",
      "ItemNo": "SERIAL2",
      "VariantCode": "",
      "Description": "C.O.S OVERDRIVE TRIMLITE",
      "LocationCode": "ASIA",
      "SalespersPurchCode": "",
      "QtyCalculated": 0.0,
      "QtyPhysInventory": 2.0,
      "Quantity": 2.0,
      "UserID": "{92012D15-CA99-4CEF-81FE-5D89B117139C}",
      "LineNo": 10000,
      "BinCode": "",
      "UnitofMeasureCode": "EA",
      "SerialNo": "",
      "LotNo": "",
      "ExpirationDate": "0001-01-01",
      "UncountedSerialsJA": [],
      "CountedSerialsJA": [
        {
          "SerialNo": "X141"
        },
        {
          "SerialNo": "X151"
        }
      ]
    }
  ],
  "Duration": "46 seconds 535 milliseconds"
}
```

#### **Explanation**
- **WriteInventoryCount_Insert**: A list of journal lines that have been processed.
  - **JournalTemplateName**: The journal template used.
  - **JournalBatchName**: The batch name of the journal.
  - **PostingDate**: The posting date of the journal entry.
  - **EntryType**: The type of entry, such as "Positive Adjmt." (Positive Adjustment).
  - **DocumentNo**: The document number for the journal entry.
  - **ItemNo**: The item number for the entry.
  - **VariantCode**: The variant code of the item, if applicable.
  - **Description**: The description of the item.
  - **LocationCode**: The location where the item is stored.
  - **QtyCalculated**: The quantity calculated by the system.
  - **QtyPhysInventory**: The physical inventory quantity that was counted.
  - **Quantity**: The final quantity for the item in the journal.
  - **UserID**: The ID of the user that processed the entry.
  - **LineNo**: The line number of the journal entry.
  - **BinCode**: The bin code associated with the entry.
  - **UnitofMeasureCode**: The unit of measure code for the item.
  - **SerialNo**: The serial number, if applicable.
  - **LotNo**: The lot number, if applicable.
  - **ExpirationDate**: The expiration date of the item, if applicable.
  - **UncountedSerialsJA**: Serial numbers not counted during the physical inventory.
  - **CountedSerialsJA**: Serial numbers that were counted.

#### **Summary**
The `WriteInventoryCount_Insert` API processes physical inventory counts into the item journal, handling both regular items and serialized items. The API records these counts into Business Central, ensuring accurate inventory tracking and adjustments.

### **Implementation Logic**
1. **Initial Validations**: 
   - Validate the existence of items and that quantities are valid.
   - Ensure that serial numbers are tracked correctly.

2. **Inserting Journal Lines**:
   - For each item, insert a new line into the item journal.
   - If serialized, track each serial number provided in the request.

3. **Handling Serial Numbers**:
   - If the item has serial numbers, validate and insert each serial number into the journal entry.

4. **Inventory Discrepancy Handling**:
   - Calculate any discrepancies between the system's calculated quantity and the physical count, adjusting the item journal accordingly.

### **Additional Considerations**
- **Serial Number Tracking**: The `SerialJA` array must be populated with accurate serial numbers for serialized items, ensuring that each serial number is tracked correctly.
- **Inventory Discrepancies**: Any differences between the calculated and physical inventory quantities are recorded and adjusted automatically in the item journal.

