# Palette's Journal - SkinGPT-4 UX/Accessibility Learnings

## 2024-11-20 - Gradio 3.24.1 Accessibility and Collapsible Disclaimers
**Learning:** Collapsing verbose, non-interactive legal or medical disclaimers inside a `gr.Accordion` defaulting to `open=False` improves focus and scannability, particularly for key diagnostic tools. Explicitly labeling `gr.Image` components ensures optimal screen reader compatibility. Additionally, using Gradio's `info` parameter to clarify how specific mathematical hyperparameters impact diagnosis and performance enhances user trust and usability.
**Action:** Always wrap long non-interactive textual content in `gr.Accordion(open=False)`, add explicit user-friendly labels to all uploaded input media elements, and supply descriptive instruction text inside `info` properties of interactive sliders.
