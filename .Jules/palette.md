# Palette's Journal - SkinGPT-4 UX/a11y Insights

## 2025-02-14 - Collapsible Disclaimers and Descriptive Inputs in Gradio 3.24.1
**Learning:** Medical AI interfaces often present long legal or clinical disclaimers that clutter the viewport and distract from the primary call to action. Wrapping these disclaimers in a collapsible `gr.Accordion` component (with `open=False`) keeps the interface clean while ensuring the legal text is still easily accessible. Removing redundant headers inside the collapsible container also saves precious vertical space.
Furthermore, Gradio 3.24.1 slider and image inputs benefit enormously from descriptive `label` and `info` properties, which aid accessibility (via screen readers) and clarify advanced parameters (such as Temperature and Beam Search) for users who might not understand deep learning jargon.
Finally, setting column scales to integer ratios (e.g., `scale=1` and `scale=2` instead of float fractions like `0.5`) ensures robust and visually consistent grid layouts in Gradio.
**Action:** Apply `gr.Accordion` for disclaimers, add meaningful `info` text to parameters, provide explicit labels to image inputs, and use integer-based column scaling.
