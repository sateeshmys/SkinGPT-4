## 2025-05-14 - Decluttering with Accordions and Accessible Labels

**Learning:** In medical AI applications with long legal disclaimers, using `gr.Accordion(open=False)` significantly improves the "above the fold" experience, allowing users to focus on the primary task (uploading images) while keeping essential information accessible. Additionally, Gradio's `info` parameter for sliders is highly effective for explaining complex model parameters to non-technical users.

**Action:** Always wrap secondary/legal text in collapsed accordions and use `info` fields to provide contextual help for technical model settings.
