flowchart LR

    Procurement["Procurement Module"]

    PO["Purchase Order"]

    Goods["Goods Receipt"]

    Inventory["Inventory Management"]

    Stock["Stock Database"]

    Reconciliation["Inventory Reconciliation"]

    Alert["Low Stock / Reorder Alert"]

    Forecast["AI Stock Forecasting"]

    Dashboard["Executive Dashboard"]

    Procurement --> PO
    PO --> Goods
    Goods --> Inventory

    Inventory --> Stock

    Stock --> Reconciliation
    Procurement --> Reconciliation

    Reconciliation --> Alert

    Stock --> Forecast
    Forecast --> Dashboard

    Inventory --> Dashboard