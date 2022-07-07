# Development Process

``` mermaid
graph LR
  A((Discovery)) ---> B{Requirements<br/>Documentation};
  B --> C((Iteration));
  C --> A;
  C --> D[Contract];
  D --> E{Wireframing,<br/>Protoyping, UI<br/>Figma};
  E --> F((Requirements<br/>Updates));
  F --> X((Client Feedback));
  X --> E;
  F --> G{Development Phase};
  G --> H((Testing));
  H --> G;
  H --> I{MVP}
```
