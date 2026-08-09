# Palette's Journal - Critical UX and Accessibility Insights

## 2025-02-12 - Medical AI Disclaimer and Settings UX
**Learning:** Medical AI interfaces often present a wall of text (disclaimers) and unexplained tuning sliders (beam search, temperature) that overwhelm patients/physicians. Wrapping long secondary texts in a collapsible accordion improves focus. Additionally, explaining parameters via `info` field hints helps demystify the machine learning parameters.
**Action:** Use `gr.Accordion` for disclaimers and define `info` parameter descriptions for interactive sliders.
