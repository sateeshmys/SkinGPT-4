## 2025-05-14 - Collapsible Disclaimers
**Learning:** Long legal disclaimers or secondary information in Gradio apps can push core interactive elements "below the fold," hindering the user experience.
**Action:** Always wrap long secondary text in a `gr.Accordion` (initially closed) to maintain focus on the main interface while keeping information accessible.
