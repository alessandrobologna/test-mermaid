# Mermaid Samples

## Flowchart Example

```mermaid
%%{init: {"flowchart": {"diagramPadding": 130}, "htmlLabels": true}}%%
flowchart TB
  Start([Start]) --> Input[Collect Input]
  Input --> Validate{Valid?}
  Validate -->|Yes| Process[Process Request]
  Validate -->|No| Retry[Ask for Fix]
  Retry --> Input
  Process --> Done([Done])
```

## Sequence Diagram Example

```mermaid
%%{init: {"htmlLabels": true, "sequence": {"diagramMarginX": 130, "diagramMarginY": 30, "bottomMarginAdj": 130}}}%%
sequenceDiagram
  participant U as User
  participant A as API
  participant D as Database

  U->>A: POST /items
  A->>D: Insert item
  D-->>A: Inserted (id)
  A-->>U: 201 Created
```
