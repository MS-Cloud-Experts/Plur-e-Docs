    
```
    [IntegrationEvent(false, false)]
    procedure OnBeforeGetSalesReportinBase64(var SalesHeader: Record "Sales Header"; var SalesDocumentType: enum "Sales Document Type"; var DocumentNo: Code[20]; var ReportID: Integer; var TextOutput: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnAfterGetSalesReportinBase64(var SalesHeader: Record "Sales Header"; var SalesDocumentType: enum "Sales Document Type"; var DocumentNo: Code[20]; var ReportID: Integer; var TextOutput: Text)
    begin
    end;
```
