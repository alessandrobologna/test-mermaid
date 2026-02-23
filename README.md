# Mermaid Samples

## Flowchart Example

```mermaid
flowchart TD
  A[Start] --> B{Is it valid?}
  B -->|Yes| C[Process]
  B -->|No| D[Fix Input]
  D --> B
  C --> E[Done]
```

### Flowchart SVG (Generated with Node Mermaid.js)

<img src="./flowchart.node.svg" alt="Flowchart SVG" height="558" />

## Sequence Diagram Example

```mermaid
sequenceDiagram
  participant User
  participant API
  participant DB

  User->>API: Create item
  API->>DB: Insert row
  DB-->>API: OK
  API-->>User: 201 Created
```

### Sequence SVG (Generated with Node Mermaid.js)

<img src="./sequence.node.svg" alt="Sequence SVG" height="423" />

## Long Vertical Flowchart Example

```mermaid
flowchart TD
  S[Step 1: Intake] --> A[Step 2: Validate Input]
  A --> B[Step 3: Normalize Data]
  B --> C[Step 4: Enrich Context]
  C --> D[Step 5: Persist Record]
  D --> E[Step 6: Trigger Notification]
  E --> F[Step 7: Archive]
  F --> G[Done]
```

### Long Vertical Flowchart SVG (Generated with Node Mermaid.js)

<img src="./flowchart-2.node.svg" alt="Long Vertical Flowchart SVG" height="878" />
