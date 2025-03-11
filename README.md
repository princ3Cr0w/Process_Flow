# Process_Flow
Niche restaruant process flow diagram
Markdown

# Restaurant Business Flow

This diagram illustrates the customer flow in a restaurant, from arrival to departure.

```mermaid
graph TD
    A[Customer Arrives] --> B{Table Available?};
    B -- Yes --> C[Seated & Menus];
    B -- No --> D[Waiting Area];
    D --> E[Table Becomes Available];
    E --> C;
    C --> F[Order Taken];
    F --> G[Order Sent to Kitchen];
    G --> H[Food Preparation];
    H --> I[Food Ready];
    I --> J[Food Served];
    J --> K[Customer Eats];
    K --> L{Finished Eating?};
    L -- Yes --> M[Bill Presented];
    L -- No --> K;
    M --> N[Payment Processed];
    N --> O[Customer Leaves];
    F --> P{Drinks Ordered?};
    P -- Yes --> Q[Drinks Prepared];
    P -- No --> G;
    Q --> J;
    G --> R{Special Requests?};
    R -- Yes --> S[Special Request Fulfilled];
    R -- No --> H;
    S --> H;
