flowchart TD

    Users["Users"]

    Application["Enterprise Operations Platform"]

    Procurement["Procurement"]
    Inventory["Inventory"]
    Assets["Asset Management"]
    Vendors["Vendor Hub"]

    Database["Operational Database"]

    Analytics["Analytics Engine"]

    Dashboard["Executive Dashboard"]

    AI["AI / ML"]

    IoT["IoT Sensors"]

    Users --> Application

    Application --> Procurement
    Application --> Inventory
    Application --> Assets
    Application --> Vendors

    Procurement --> Database
    Inventory --> Database
    Assets --> Database
    Vendors --> Database

    Database --> Analytics

    Analytics --> Dashboard

    Database --> AI
    AI --> Dashboard

    IoT --> AI
    IoT --> Assets

    Dashboard --> Users
    