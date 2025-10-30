```mermaid
graph TD
    A[Veřejná správa ČR]
    A --> B[Státní správa]
    A --> C[Samospráva]

    B --> B1[Přímá státní správa]
    B --> B2[Nepřímá státní správa (Přenesená působnost)]

    B1 --> B1a[Vláda ČR]
    B1a --> B1b[Ministerstva]
    B1a --> B1c[Další ústřední správní úřady (např. ČSÚ, ERÚ)]
    B1 --> B1d[Prezident republiky]
    B1 --> B1e[Územní správní úřady (např. Finanční úřady, KHS)]

    C --> C1[Územní samospráva]
    C --> C2[Zájmová / Profesní samospráva (např. ČAK, ČLK)]

    C1 --> C1a[Kraje (VÚSC)]
    C1a --> C1a1[Zastupitelstvo kraje (volený orgán)]
    C1a1 --> C1a2[Rada kraje (výkonný orgán)]
    C1a2 --> C1a3[Hejtman]
    C1a1 --> C1a4[Krajský úřad]
    
    C1 --> C1b[Obce (ZÚSC)]
    C1b --> C1b1[Zastupitelstvo obce (volený orgán)]
    C1b1 --> C1b2[Rada obce (výkonný orgán)]
    C1b2 --> C1b3[Starosta / Primátor]
    C1b1 --> C1b4[Obecní / Městský úřad / Magistrát]
    
    %% Propojení přenesené působnosti
    B2 -.-> C1a4
    B2 -.-> C1b4

    %% Styling
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bdf,stroke:#333
    style C fill:#bdf,stroke:#333
    style B1 fill:aliceblue
    style B2 fill:aliceblue
    style C1 fill:lightyellow
    style C2 fill:lightyellow
    style C1a fill:#fef
    style C1b fill:#fef
```
