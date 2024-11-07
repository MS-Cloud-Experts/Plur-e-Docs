Primera version LP con Script de BC, revisar errores y mejorar el paso a paso

# Warehouse Shipment Process Analysis

## Step-by-Step Process
1. Initiated warehouse shipment creation from Sales Order page
   - Warehouse Shipment Header created (ID: WHSE SHIP-00046)

2. Item Selection Process
   - Opened Warehouse Shipment form
   - Attempted to select Item No. through lookup
   - Viewed Item Card details
   - Closed Item Card

3. Pick Creation Process
   - Initiated "Create Pick" action
   - Pick activity created (ID: WHSE PICK-00048)
   - Opened Warehouse Pick Lines view

4. License Plate Assignment Process
   - Accessed Warehouse Pick (WHSE PICK-00048)
   - Attempted to view optimal LP eligible items
   - Opened LP Optimal Selection window
   - First LP assignment attempt:
     - Selected LP-00027
     - Assignment failed
   - Second LP assignment attempt:
     - Viewed all eligible License Plates
     - Selected LP-00035
     - Assignment failed

5. Final Action
   - Navigated to Plur-E License Plates List
   - Attempted to select different rows in the list

## Errors and Issues Encountered

1. First License Plate Assignment Error
   - Attempted to assign LP-00027
   - System showed an error dialog (specific error message not recorded)

2. Second License Plate Assignment Error
   - Attempted to assign LP-00035
   - System returned message: "LP-00035 was Not Assigned"

## System Navigation Path
- Sales Order → Warehouse Shipment → Item Selection → Pick Creation → License Plate Assignment → License Plates List
