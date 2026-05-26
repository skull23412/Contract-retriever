# CCNL Data Extractor

Project for extracting structured payroll data from Italian CCNL documents.

Target fields:

- minimo contrattuale
- contingenza
- elemento distinto della retribuzione / EDR
- divisore orario
- mensilita

Planned pipeline:

1. Parse PDF text and tables.
2. Split documents into article and table chunks.
3. Tag chunks by semantic field.
4. Retrieve relevant chunks with keyword and vector search.
5. Ask a local Ollama model to return structured JSON from retrieved context.

