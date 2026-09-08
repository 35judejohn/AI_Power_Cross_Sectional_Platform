```mermaid
flowchart TD

    Register["Asset Registration"]
    AssetDB["Asset Database"]
    Assignment["Asset Assignment"]
    Location["Asset Location"]
    Maintenance["Maintenance History"]

    Service["Service Schedule"]
    Alert["Service / Replacement Alert"]
    IoT["IoT Sensor Data"]
    Predictive["Predictive Maintenance Model"]
    Dashboard["Executive Dashboard"]

    Register --> AssetDB
    AssetDB --> Assignment
    AssetDB --> Location
    AssetDB --> Maintenance
    AssetDB --> Service

    Service --> Alert

    Maintenance --> Predictive
    IoT --> Predictive

    Predictive --> Alert

    AssetDB --> Dashboard
    Maintenance --> Dashboard
    Predictive --> Dashboard
