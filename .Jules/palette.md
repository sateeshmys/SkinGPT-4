# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-02-20 - Gradio 3.24.1 UX Patterns for Medical AI
**Learning:** Collapsing secondary text, such as a long medical disclaimer, into a `gr.Accordion` is crucial for prioritizing core interactive elements in Gradio 3.24.1. Also, utilizing integer scales for columns (like `scale=1` and `scale=2`) instead of floats preserves layout ratios reliably, and descriptive `info` text for model parameters aids user understanding.
**Action:** Use collapsible accordions with `open=False` for disclaimers, apply explicit `label` parameters on `gr.Image`, employ `variant="secondary"` for non-primary buttons, and provide descriptive `info` help text for sliders in Gradio form elements.
