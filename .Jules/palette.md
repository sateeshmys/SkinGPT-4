# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-02-18 - Collapsible Medical Disclaimers in Gradio
**Learning:** Medical AI applications often require extensive disclaimers. Displaying these as raw, long paragraphs of text clutters the interface and distracts from core interactions. Using a collapsible container improves layout focus and user experience.
**Action:** Wrap long secondary or legal text in a collapsible `gr.Accordion` container defaulting to `open=False`. Remove redundant headers inside the text block to maintain high information density without visual noise.

## 2025-02-18 - Integer-Based Column Scaling in Gradio 3.24.1
**Learning:** In older versions of Gradio (like 3.24.1), providing float values for column scaling (such as `scale=0.5`) is not supported and can cause layout inconsistencies. Columns require integer scaling weights.
**Action:** To maintain a 1:2 layout ratio, set `scale=1` for the smaller column and `scale=2` for the larger column.

## 2025-02-18 - Descriptive Label and Info Fields for Gradio Form Components
**Learning:** In medical AI applications, user interface parameters like 'Beam Search Numbers' or 'Temperature' are opaque and confusing to patients or clinical end-users. Lacking info/help text increases user uncertainty.
**Action:** Use the `info` parameter in Gradio components (such as sliders) to clearly and concisely explain how parameter adjustments affect generation quality, creativity, latency, and determinism.

## 2025-02-18 - Screen Reader Accessibility for Image Uploads
**Learning:** Image upload components in Gradio often lack explicit labels, making them inaccessible to screen readers and causing confusion about user intent.
**Action:** Always provide an explicit, descriptive `label` parameter (e.g. "Upload Skin Image") to the `gr.Image` component to ensure screen reader accessibility and clear user intent.
