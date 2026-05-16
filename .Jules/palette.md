## 2025-05-15 - [Layout & Disclosure Patterns]
**Learning:** In Gradio 3.24.1, 'scale' values for layout components must be integers to ensure consistent rendering and avoid warnings. Additionally, long secondary content like medical disclaimers should always be wrapped in a collapsed 'gr.Accordion' to maintain focus on core interactive elements 'above the fold'.
**Action:** Always use integer scales (e.g., 1:2) for responsive layouts and prioritize 'gr.Accordion' for decluttering long textual sections.
