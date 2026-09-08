```mermaid
flowchart TD

    Vendor["Supplier"]

    Registration["Supplier Registration"]

    Documents["Business Documents"]

    CAC["CAC Verification"]

    TIN["TIN Verification"]

    Bank["Bank Account Name Match"]

    Certification["Certification Verification"]

    Rules["Verification Rules Engine"]

    Risk["Risk Scoring"]

    Reviewer["Human Reviewer"]

    Status["Vendor Status"]

    Verified["VERIFIED"]
    Flagged["FLAGGED"]
    Rejected["REJECTED"]

    Vendor --> Registration
    Registration --> Documents

    Registration --> CAC
    Registration --> TIN
    Registration --> Bank
    Registration --> Certification

    CAC --> Rules
    TIN --> Rules
    Bank --> Rules
    Certification --> Rules

    Documents --> Rules

    Rules --> Risk

    Risk --> Reviewer

    Reviewer --> Status

    Status --> Verified
    Status --> Flagged
    Status --> Rejected
