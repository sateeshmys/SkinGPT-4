## 2025-05-10 - Accordion Disclaimers and Slider Micro-Copy in Gradio
**Learning:** Collapsing lengthy medical disclaimers into a closed `gr.Accordion` declutters the interface and keeps key CTA controls above the fold. Adding explicit labels to `gr.Image` and `info` text to sliders clarifies expected model behavior for clinical/technical parameters like temperature and beam search.
**Action:** Always wrap disclaimers/long terms in `gr.Accordion(open=False)` and provide `info` text for model parameters in Gradio web interfaces.
