 
```
    [IntegrationEvent(false, false)]
    procedure OnBeforeVoidPayment(CustomerNo: Code[50]; PostedDocNo: Text; PostingDate: Date; DocumentDate: Date; Amount: Decimal; TransactionNo: Text; IsPosted: Boolean; var OutPut: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetGenJournalBatchJson(var OutPut: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetPaymentMethods(var OutPut: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforePaymentOrders(CustomerNo: Code[50]; PostedDocNo: Text; PostingDate: Date; DocumentDate: Date; Amount: Decimal; TransactionNo: Text; JournalTemplateName: Code[10]; JournalBatchName: Code[10]; ParamsJToken: JsonToken; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeUnpaidOrders(CustomerNo: Code[50]; var Output: Text; var IsHandled: Boolean)
    begin
    end;
```
