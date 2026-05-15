## 2025-05-14 - Collapsible Disclaimers for Medical AI
**Learning:** Medical AI applications often require long legal disclaimers that push the actual interactive components (like image upload and chat) "below the fold," hurting the initial user experience.
**Action:** Always wrap long secondary text (like disclaimers) in collapsible 'gr.Accordion' components to maintain focus on the main interactive elements 'above the fold'.

## 2025-05-14 - Gradio Accessibility for Image Inputs
**Learning:** The default 'gr.Image' component without a label can be confusing for screen readers and new users in specialized diagnostic apps.
**Action:** Always provide explicit 'label' parameters for 'gr.Image' components (e.g., 'Upload Skin Image') to ensure screen reader accessibility and clear user intent.
