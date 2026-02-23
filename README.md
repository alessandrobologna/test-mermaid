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
