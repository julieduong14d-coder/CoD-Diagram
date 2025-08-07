flowchart LR
  subgraph MP [Major Powers]
    USA(["USA"])
    CHN(["China"])
    RUS(["Russia"])
  end

  subgraph AL [Alliances]
    WA(["Western Allies<br/>(NATO, US–Japan, AUKUS, Five Eyes)"])
    SCO(["SCO<br/>(Shanghai Cooperation O.)"])
    BRICS(["BRICS"])
    CSTO(["CSTO<br/>(Collective Security Treaty O.)"])
  end

  subgraph HS [Helios System]
    HEL(["Helios"])
    NEU(["Neutral Countries<br/>(Switzerland, Austria, Ireland, …)"])
  end

  %% align columns
  MP --> AL
  AL --> HS

  %% details
  USA --> WA
  CHN --> SCO
  CHN --> BRICS
  RUS --> CSTO
  RUS --> BRICS

  USA --> HEL
  CHN --> HEL
  RUS --> HEL

  HEL --> NEU
