---
config:
  theme: base
  themeVariables:
    primaryColor: '#f0f0f0'
    primaryTextColor: '#333'
    primaryBorderColor: '#999'
    lineColor: '#666'
    sectionBkgColor: '#f5f5f5'
    altSectionBkgColor: '#e0e0e0'
    gridColor: '#ddd'
    background: '#f0f0f0'
    mainBkg: '#f0f0f0'
    secondBkg: '#f0f0f0'
---
flowchart TD
 subgraph REC["💡 Рекомендації"]
        F["💡 Рек. C"]
        G["💡 Рек. G"]
        H["💡 Рек. GPT"]
        X["📋 Диф Саммері"]
  end
 subgraph DIAL["📞 Діалоги"]
        I["📞 Діалог 1"]
        J["📞 Діалог 2"]
        K["📞 Діалог 3"]
        Z["📋 Диф Саммері"]
  end
 subgraph DEMO["👥 Демо діалоги"]
        M["👥 Демо 1"]
        N["👥 Демо 2"]
        O["👥 Демо 3"]
        Q["📋 Диф Саммері"]
  end
    A["🗣️ Початкова<br>розмова"] --> C["Claude"] & D["Gemini"] & E["ChatGPT"]
    C --> B1{"📝 Саммарі<br>Claude"}
    D --> B2{"📝 Саммарі<br>Gemini"}
    E --> B3{"📝 Саммарі<br>ChatGPT"}
    B1 --> F
    B2 --> G
    B3 --> H
    F --> I
    G --> J
    H --> K
    I --> L{"👥 Демо-тренди"}
    J --> L
    K --> L
    L --> M & N & O
    M --> P["📊 Обовідання"]
    N --> P
    O --> P
    style X fill:#ffecb3,stroke:#f57f17,stroke-width:2px
    style Z fill:#ffecb3,stroke:#f57f17,stroke-width:2px
    style Q fill:#ffecb3,stroke:#f57f17,stroke-width:2px
    style A fill:#e1f5fe,stroke:#0277bd,stroke-width:2px
    style B1 fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
    style B2 fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
    style B3 fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
    style L fill:#e8f5e8,stroke:#388e3c,stroke-width:2px
    style P fill:#ffebee,stroke:#c2185b,stroke-width:3px
    style REC stroke:#666,stroke-width:2px,stroke-dasharray: 5 5,fill:transparent
    style DIAL stroke:#666,stroke-width:2px,stroke-dasharray: 5 5,fill:transparent
    style DEMO stroke:#666,stroke-width:2px,stroke-dasharray: 5 5,fill:transparent
