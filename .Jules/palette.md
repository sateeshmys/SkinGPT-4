## 2025-05-14 - [Gradio Disclaimer Accordion Pattern]
**Learning:** In medical AI applications, long disclaimers can dominate the UI, pushing primary interactive components like image uploaders and chat interfaces 'below the fold'. Wrapping these in a collapsed `gr.Accordion` significantly improves initial focus and UX flow.
**Action:** Always use `gr.Accordion` for lengthy secondary content (legal disclaimers, license info, detailed documentation) in Gradio interfaces to maintain a clean, action-oriented primary view.
