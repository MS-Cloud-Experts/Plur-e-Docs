[IntegrationEvent(false, false)]
    internal procedure OnBeforeGetSalesPersonsList(var SalesPeople: Record "Salesperson/Purchaser"; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnAfterGetItemProcedure(var tableNo1: Integer; var tableNo2: Integer; var tableNo3: Integer; var tableNo4: Integer; var JsonObject: JsonObject; var Output: Text; var pageSizeText: Text)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeDeleteDocument(SalesPerson: Text; DocumentType: Text; DocumentNo: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItemProcedure(var tableNo1: Integer; var tableNo2: Integer; var tableNo3: Integer; var tableNo4: Integer; var JsonObject: JsonObject; var Output: Text; var pageSizeText: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGet_ItemReclassJournal(JournalBatchName: Code[10]; JournalTemplateName: Code[10]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGet_ItemTransfersBatch(var Ouput: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetCustomer(No: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetCustomersList(pageSizeText: Text; salesPersonCode: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItem(ItemNo: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItemCategoriesList(pageSizeText: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItemIdentifier(Code: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItemInfo(ItemNo: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItemInventoryByLocation(ItemNo: Code[20]; LocationFilter: Code[10]; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetItems(pageSizeText: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetSalesCount(pageSizeText: Text; SalesPerson: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetSalesCountWhitoutSalesPerson(pageSizeText: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetSalesOrders(DocumentType: Text; No: Text; pageSizeText: Text; position: Text; SalesPerson: Text; var Output: Text; var IsHandled: Boolean)
    begin
    end;

    [IntegrationEvent(false, false)]
    procedure OnBeforeGetSalesPerson(CodeSP: Code[20]; var Output: Text; var IsHandled: Boolean)
    begin
    end;