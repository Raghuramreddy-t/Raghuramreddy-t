%%{init: {
  "theme": "base",
  "themeVariables": {
    "background": "#050816",
    "primaryColor": "#0B1020",
    "primaryTextColor": "#F8FAFC",
    "primaryBorderColor": "#22D3EE",
    "lineColor": "#8B5CF6",
    "secondaryColor": "#111827",
    "tertiaryColor": "#1E293B",
    "fontFamily": "Inter, Segoe UI, Arial"
  }
}}%%

flowchart LR
    A["Delivery Signals"] --> B["Runtime State"]
    B --> C["Security Context"]
    C --> D["Ownership Metadata"]
    D --> E["Governance Rules"]
    E --> F["Operational Cognition"]
    F --> G["Human-Governed Decisions"]

    X["EOCS<br/>Enterprise Operational Cognition System"] -. connects .- A
    X -. correlates .- B
    X -. governs .- C
    X -. reasons over .- D
    X -. enforces .- E
    X -. explains .- F
    X -. supports .- G

    classDef signal fill:#082F49,stroke:#38BDF8,color:#F8FAFC,stroke-width:2px;
    classDef runtime fill:#0B1020,stroke:#22D3EE,color:#F8FAFC,stroke-width:2px;
    classDef security fill:#1E1B4B,stroke:#8B5CF6,color:#F8FAFC,stroke-width:2px;
    classDef gov fill:#581C87,stroke:#A855F7,color:#F8FAFC,stroke-width:2px;
    classDef cognition fill:#111827,stroke:#F8FAFC,color:#F8FAFC,stroke-width:2px;
    classDef eocs fill:#020617,stroke:#22D3EE,color:#F8FAFC,stroke-width:3px;

    class A signal;
    class B runtime;
    class C security;
    class D gov;
    class E gov;
    class F cognition;
    class G cognition;
    class X eocs;
