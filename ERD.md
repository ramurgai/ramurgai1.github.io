# Card Shop Stuff:

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
    string card_number "Card Number"
    }

    SALE {
        string id PK "Sale ID"
        date date "Sale Date"
        string customerid FK "Customer ID"
        string productid FK "Product ID"
        int quantity "Quantity Sold"
    }
    INVENTORY {
    string productid FK "Product ID"
    int stock "Current stock available"

    }