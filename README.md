```mermaid
graph TD
    %% Hlavní část modelu
    B[Veřejná správa ČR<br><b>Spojený model</b>]:::main

    B --> C[<b>Státní správa</b>]:::statni
    B --> D[<b>Samospráva</b>]:::samosprava
    B --> E[<b>Ostatní Veřejná správa</b>]:::ostatni

    %% Státní správa detailněji
    C --> C1[Ústřední orgány]:::ustredni
    C1 --> C1a(Vláda ČR):::vlada
    C1 --> C1b(Ministerstva):::ministerstva
    C1 --> C1c(Ostatní ÚSÚ):::usu

    C --> C2[Územní orgány]:::uzemni
    C2 --> C2a(Finanční úřady):::financni
    C2 --> C2b(Celní správa):::celni
    C2 --> C2c(ČSSZ):::cssz

    C --> C3[Nepřímý výkon]:::neprimy
    C3 --> C3a(Přenesená působnost):::prenesena
    C3a -.-> D1(Krajské úřady):::krajsky
    C3a -.-> D2(Obecní/Městské úřady):::obecni
    
    %% Samospráva detailněji
    D --> D1[Územní samospráva<br>Kraje]:::kraje
    D --> D2[Územní samospráva<br>Obce]:::obce
    D --> D3[Zájmová samospráva]:::zajmova

    D1 --> D1a(Zastupitelstvo kraje):::zastupitelstvoK
    D1 --> D1b(Krajský úřad):::uradK

    D2 --> D2a(Zastupitelstvo obce/města):::zastupitelstvoO
    D2 --> D2b(Obecní/Městský úřad):::uradO
    D2b --> D2c(Obce s ORP):::orp

    D3 --> D3a(Vysoké školy):::vysokeSkoly %% <-- PŘIDANÝ UZEL

    %% Ostatní veřejná správa
    E --> E1(Profesní komory):::komory
    E --> E2(Veřejné fondy):::fondy

    %% Stylování uzlů + černý text
    classDef main fill:#baf7ba,stroke:#333,stroke-width:3px,color:#111
    classDef split fill:#fffbe6,stroke:#f5b041,stroke-width:2px,color:#111
    classDef statni fill:#ffe5d9,stroke:#e17055,stroke-width:2px,color:#111
    classDef samosprava fill:#d0e6ff,stroke:#0984e3,stroke-width:2px,color:#111
    classDef ostatni fill:#fff8dc,stroke:#636e72,stroke-width:2px,color:#111

    classDef ustredni fill:#f9d8a5,stroke:#e17055,color:#111
    classDef vlada fill:#ffb366,stroke:#e67e22,color:#111
    classDef ministerstva fill:#ffd699,stroke:#e17055,color:#111
    classDef usu fill:#ffe5b4,stroke:#b9770e,color:#111

    classDef uzemni fill:#e3f2fd,stroke:#0984e3,color:#111
    classDef financni fill:#cfd8dc,stroke:#636e72,color:#111
    classDef celni fill:#b2ebf2,stroke:#00bcd4,color:#111
    classDef cssz fill:#e1bee7,stroke:#8e24aa,color:#111

    classDef neprimy fill:#ffd6e0,stroke:#d7263d,color:#111
    classDef prenesena fill:#ffe6cc,stroke:#f6b93b,stroke-dasharray: 5 5,color:#111

    classDef krajsky fill:#a3d9a5,stroke:#009432,color:#111
    classDef obecni fill:#b2bec3,stroke:#636e72,color:#111

    classDef kraje fill:#d4fc79,stroke:#27ae60,color:#111
    classDef obce fill:#f6e58d,stroke:#f9ca24,color:#111
    classDef zajmova fill:#f3a683,stroke:#c44569,color:#111
    classDef zastupitelstvoK fill:#b8e994,stroke:#27ae60,color:#111
    classDef uradK fill:#78e08f,stroke:#009432,color:#111
    classDef zastupitelstvoO fill:#fdcb6e,stroke:#f9ca24,color:#111
    classDef uradO fill:#ffeaa7,stroke:#f9ca24,color:#111
    classDef orp fill:#fab1a0,stroke:#e17055,color:#111
    classDef vysokeSkoly fill:#f7c8b3,stroke:#c44569,color:#111 %% <-- PŘIDANÝ STYL

    classDef komory fill:#dfe6e9,stroke:#636e72,color:#111
    classDef fondy fill:#c7ecee,stroke:#00b894,color:#111

    %% Zvýraznění klíčových vztahů
    linkStyle 13 stroke:#27ae60,stroke-width:2px,stroke-dasharray: 5 5
    linkStyle 14 stroke:#f9ca24,stroke-width:2px,stroke-dasharray: 5 5
```
