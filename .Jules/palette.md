## 2025-05-14 - Decluttering with Accordions and Gradio 3.24.1 Constraints
**Learning:** For interfaces with legally required but space-consuming content like medical disclaimers, using `gr.Accordion` (available in Gradio 3.24.1) effectively declutters the UI while keeping information accessible. Additionally, `gr.Column` scales must be integers in this version to avoid layout warnings and instability.
**Action:** Default to collapsed accordions for long secondary text. Ensure all layout scales are integers when working with older Gradio versions.
