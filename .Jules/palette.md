## 2025-05-15 - Medical AI UX Patterns in Gradio

**Learning:** Medical AI applications often have long legal disclaimers and technical parameters (like beam search or temperature) that can overwhelm the user. Using collapsible accordions for disclaimers and 'info' tooltips for sliders maintains a clean interface while providing necessary context and accessibility.

**Action:** Always wrap long secondary text in 'gr.Accordion(open=False)' and use the 'info' parameter in 'gr.Slider' to explain complex settings. Ensure 'gr.Image' components have explicit 'label' parameters for screen readers.
