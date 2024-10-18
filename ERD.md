``` mermaid
erDiagram
    PRODUCT ||--|{ SALE: "is sold in"
    PRODUCT ||--|| INVENTORY: "is tracked in"
    CUSTOMER ||--o{ SALE: makes
    PRODUCT{
        string productid PK "Unique product ID"
        string card "Card Name"
        float price "Price"   
    }

    CUSTOMER {
    string customerid PK "Unique Customer ID"
    string name "Customer Name"
    string name "Email address"
    int card_number 
    }

    SALE {
        string id PK "Sale ID"

    }