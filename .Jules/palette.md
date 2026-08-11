# Palette Journal

## 2025-02-17 - Gradio 3.24.1 Layout and Disclaimer Enhancements
**Learning:** Collapsing extensive secondary text like medical disclaimers in a `gr.Accordion` declutters the workspace, allowing users to focus on primary interactive components. In Gradio 3.24.1, scale parameters must be integers to render correctly, so a 1:2 layout is best achieved with `scale=1` and `scale=2` columns. Using `info` fields for medical parameters clarifies how adjustment affects diagnostic output.
**Action:** Always wrap long disclaimer text in a collapsed `gr.Accordion(open=False)`, set integer values for column scales, use explicit labels/info for input elements, and use secondary variant styles for non-primary actions.
