## 2025-05-15 - Medical Disclaimer UX Pattern
**Learning:** In medical AI applications, long disclaimers can overwhelm the user and distract from the main interface. Encapsulating them in a collapsible `gr.Accordion` (defaulting to closed) maintains legal compliance while significantly improving initial focus and layout clarity.
**Action:** Use `gr.Accordion(label="Medical Disclaimer", open=False)` for extensive secondary text.

## 2025-05-15 - Parameter Clarity in Gradio
**Learning:** Technical parameters like 'Temperature' or 'Beam Search' are often obscure to non-expert users. Using the `info` parameter in `gr.Slider` to explain the real-world impact (e.g., creativity vs. determinism, quality vs. latency) provides immediate interaction feedback and improves usability.
**Action:** Always provide concise `info` text for model-specific parameters.
