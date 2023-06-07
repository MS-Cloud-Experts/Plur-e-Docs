**Request:**
```
{
  "ProcessMethod": "GetGenJournalBatchJson",
  "Parameters": []
}
```

**Output:**
```
[
  {
    "Name": "PAYMENT",
    "Description": "Payments",
    "Batch": [
      {
        "Name": "BANK",
        "Description": "Bank payments",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "",
        "BalAccountNo": "WWB-OPERATING",
        "BalAccountType": "Bank Account"
      },
      {
        "Name": "BANK CONV",
        "Description": "Payment Export using Bank Data Conversion Service",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "GJNL-PMT",
        "BalAccountNo": "WWB-TRANSFERS",
        "BalAccountType": "Bank Account"
      },
      {
        "Name": "CASH",
        "Description": "Cash receipts and payments",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "GJNL-PMT",
        "BalAccountNo": "11200",
        "BalAccountType": "G/L Account"
      },
      {
        "Name": "GENERAL",
        "Description": "GENERAL",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "GJNL-PMT",
        "BalAccountNo": "",
        "BalAccountType": "G/L Account"
      },
      {
        "Name": "GIRO",
        "Description": "Giro payments",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "GJNL-PMT",
        "BalAccountNo": "GIRO",
        "BalAccountType": "Bank Account"
      },
      {
        "Name": "PMT REG",
        "Description": "Bank Reconciliation",
        "CopytoPostedJnlLines": false,
        "PostingNoSeries": "",
        "NoSeries": "GJNL-PMT",
        "BalAccountNo": "WWB-OPERATING",
        "BalAccountType": "Bank Account"
      }
    ]
  }
]
```
