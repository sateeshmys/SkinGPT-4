## 2025-05-15 - Gradio 3.24.1 Layout Constraints
**Learning:** In Gradio 3.24.1, `gr.Column(scale=...)` must use integer values. Using float values like `0.5` causes a `UserWarning` and can lead to inconsistent layouts. Additionally, this version lacks `gr.Info`, so `info` parameters in components like `gr.Slider` or `gr.update` should be used for guidance.
**Action:** Always ensure `scale` values are integers when working with older Gradio versions and use component-level `info` or `label` for descriptive text.

## 2025-05-15 - Progressive Disclosure with Accordions
**Learning:** For medical or technical applications with long legal disclaimers, wrapping them in a `gr.Accordion` (closed by default) significantly improves the user experience by prioritizing the main interaction area ("above the fold") while keeping the information accessible.
**Action:** Use `gr.Accordion` to declutter interfaces that require large blocks of secondary text.
