## 2025-05-15 - Optimizing UI Real Estate in Medical AI Applications
**Learning:** In medical AI applications with long mandatory disclaimers, placing them directly in the main layout pushes critical interactive elements (like image uploaders) below the fold, degrading the initial user experience. Gradio's `gr.Accordion` is an effective pattern for maintaining legal compliance while keeping the UI clean and focused on user action.
**Action:** Always wrap long secondary text or legal disclaimers in a collapsed `gr.Accordion` by default to prioritize primary user tasks.
