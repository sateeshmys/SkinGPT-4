## 2025-05-15 - Medical AI UX Patterns
**Learning:** In medical AI applications, users benefit from immediate context on diagnostic parameters (like beam search or temperature) and a decluttered interface that prioritizes the interaction area over long legal disclaimers. Explicit labels on image upload components are critical for accessibility in healthcare tools.
**Action:** Always wrap long disclaimers in `gr.Accordion`, use `info` fields for parameter explanation, and ensure `gr.Image` has a clear `label`.
