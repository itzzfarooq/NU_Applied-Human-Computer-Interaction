# Chapter 8 Mind Map

```
                     ┌─────────────────────────────────────────────────────┐
                     │    IMPLEMENTATION SUPPORT (Ch 8)                   │
                     │    From hardware to conceptual architecture        │
                     └─────────────────────────────────────────────────────┘
                                        │
                  ┌─────────────────────┼─────────────────────┐
                  │                     │                     │
                  ▼                     ▼                     ▼
         ┌────────────────┐   ┌────────────────┐   ┌─────────────────┐
         │ WINDOWING      │   │ PROGRAMMING    │   │ INTERACTION     │
         │ SYSTEMS        │   │ PARADIGMS      │   │ TOOLKITS        │
         │ (Low-level)    │   │ (Input handling)│   │ (Widgets)       │
         └────────────────┘   └────────────────┘   └─────────────────┘
                  │                     │                     │
            ┌─────┴─────┐          ┌─────┴─────┐          ┌────┴────┐
            │           │          │           │          │         │
            ▼           ▼          ▼           ▼          ▼         ▼
      ┌────────┐ ┌────────┐  ┌────────┐ ┌────────┐  ┌──────┐ ┌──────┐
      │Device  │ │Resource│  │Read-   │ │Notifica│  │ AWT  │ │Swing │
      │Indep-  │ │Sharing │  │Eval    │ │tion    │  │(nativ│ │(on   │
      │endence │ │(multip │  │Loop    │ │(call-  │  │ call-│ │AWT,  │
      │        │ │le apps)│  │(repeat→│ │backs)  │  │backs)│ │MVC)  │
      │        │ │        │  │ case)  │ │        │  │      │ │      │
      │Image   │ │3 Archs │  │        │ │        │  │      │ │      │
      │models  │ │App/Kern│  │Modal→ │ │Non-mod │  └──────┘ └──────┘
      │Pixels  │ │/Separat│  │Easy    │ │→Easy   │
      └────────┘ └────────┘  └────────┘ └────────┘

         ┌─────────────────────────────────────────────────────────────┐
         │                    UIMS + ARCHITECTURES                    │
         │                (Conceptual organization)                   │
         └─────────────────────────────────────────────────────────────┘
                                    │
              ┌─────────────────────┼─────────────────────┐
              │                     │                     │
              ▼                     ▼                     ▼
      ┌──────────────┐    ┌──────────────┐    ┌──────────────┐
      │   SEEHEIM    │    │  MVC         │    │  PAC         │
      │              │    │  (Model-     │    │  (Abstractn- │
      │Presentation │    │   View-      │    │   Present-   │
      │      ↔       │    │   Controlr)  │    │   Control)   │
      │Dialogue Ctrl │    │              │    │              │
      │      ↔       │    │ Pipeline:   │    │ Hierarchical │
      │Functionality │    │ I→C→M→V→O   │    │ Control cmmc │
      │              │    │ BUT C talks │    │ I/O unified  │
      │ + Switch     │    │ to V in prc │    │ in Presenttn │
      │(rapid sd bk) │    │              │    │              │
      └──────────────┘    └──────────────┘    └──────────────┘

      ┌────────────────────────────────────────────────────────────┐
      │  IMPLEMENTATION TECHNIQUES for Dialogue Controller        │
      │  State diagrams │ Grammars │ Events │ Declarative         │
      │  Constraints (ALV) │ Graphical spec (VB, Dreamweaver)    │
      └────────────────────────────────────────────────────────────┘
```

