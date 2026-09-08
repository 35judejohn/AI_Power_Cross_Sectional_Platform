```mermaid
flowchart LR

    Employee["Employee"]
    Requisition["Purchase Requisition"]
    Approval["Approval Workflow"]
    RFQ["RFQ / Supplier Quotations"]
    VendorCheck["Vendor Verification"]
    Selection["Supplier Selection"]
    PO["Purchase Order"]
    Receipt["Goods Receipt"]
    Inventory["Inventory"]
    Dashboard["Executive Dashboard"]

    Employee --> Requisition
    Requisition --> Approval
    Approval --> RFQ

    RFQ --> VendorCheck
    VendorCheck --> Selection

    Selection --> PO
    PO --> Receipt
    Receipt --> Inventory

    Requisition --> Dashboard
    PO --> Dashboard
    Receipt --> Dashboard
    
