# Redacted Architecture Diagram

This diagram describes the public-safe system shape without exposing production source, private storage paths, credentials, vendor records, or internal workflow details.

```mermaid
flowchart LR
  Operator["Operator"]
  ProjectUI["Project workspace"]
  Inputs["Structured synthetic inputs"]
  Uploads["Reference asset upload"]
  Prompt["Prompt assembly service"]
  AI["Server-side AI generation"]
  Background["Generated background layer"]
  Composer["Deterministic composition engine"]
  Exports["PNG/PDF export"]
  Review["Read-only review link"]
  Storage["Private storage boundary"]

  Operator --> ProjectUI
  ProjectUI --> Inputs
  ProjectUI --> Uploads
  Inputs --> Prompt
  Uploads --> Storage
  Prompt --> AI
  AI --> Background
  Inputs --> Composer
  Background --> Composer
  Storage --> Composer
  Composer --> Exports
  Composer --> Review
```

## Boundary Notes

- API keys stay server-side.
- Uploaded assets stay inside the private storage boundary.
- Public examples use synthetic products, synthetic partners, and placeholder event details.
- The generated image is only one layer. Final copy, logo placement, product framing, export dimensions, and review rules are deterministic.

