## 2025-05-15 - [Gradio UI De-cluttering]
**Learning:** In medical/research AI applications, mandatory disclaimers and large parameter sets can clutter the UI, pushing main interaction elements "below the fold".
**Action:** Use `gr.Accordion` (available in Gradio 3.x) to collapse secondary information like disclaimers, and use the `info` parameter in sliders/inputs to provide contextual help without adding extra visual labels.
