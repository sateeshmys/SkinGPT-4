## 2024-08-12 - Medical Application Disclaimer Layout
**Learning:** Medical applications often require extensive, legally binding disclaimers. Displaying these in full-text by default severely pushes down critical interactive UI components, leading to a cluttered interface and high cognitive load. Encapsulating the disclaimer in a collapsible `gr.Accordion` defaults to a clean interface while maintaining accessibility.
**Action:** Always wrap long secondary or legal disclaimers in `gr.Accordion(label="Medical Disclaimer", open=False)` and remove any internal redundant headers.

## 2024-08-12 - Gradio Layout Scaling Constraints
**Learning:** In older Gradio versions like 3.24.1, using float scales (e.g., `scale=0.5`) on Column layouts can lead to unexpected sizing, as Gradio prefers integer-based scale ratios.
**Action:** Define a clean visual hierarchy and maintain a 1:2 layout ratio by specifying `scale=1` for the smaller control column and `scale=2` for the larger display/chatbot column.
