## 2025-05-15 - [Gradio 3.24.1 Layout Constraints]
**Learning:** In Gradio 3.24.1, `gr.Column` scale values must be integers (e.g., 1 instead of 0.5) to avoid `UserWarning` and potential layout breakage. Additionally, long textual content like medical disclaimers should be wrapped in `gr.Accordion` to maintain focus on primary interactive elements.
**Action:** Always use integer scales for columns and use `gr.Accordion` to group or collapse secondary information in this version of Gradio.
