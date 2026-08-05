# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-02-19 - Medical App Interface Optimization in Gradio 3.24.1
**Learning:**
- Visual clutter from lengthy legal or medical disclaimers reduces focus on primary diagnostic actions (e.g., image upload and model chatting). Encapsulating disclaimers in a collapsible component (such as `gr.Accordion`) maintains regulatory compliance without sacrificing usability.
- Explicit accessibility properties (like labels and information tooltips) are critical in medical AI applications. Slide parameters like "Temperature" and "Beam Search" can be intimidating or confusing without descriptive helper texts explaining their exact effect on generation randomness or search breadth.
- Establishing visual hierarchy through button variants (e.g., main primary action vs secondary cleanup action) and column-based layout scaling (1:2 ratio) provides a clean, professional, and accessible diagnostic dashboard.

**Action:**
- Group medical disclaimers under collapsible panels (`gr.Accordion(open=False)`).
- Provide descriptive `info` and `label` properties for all inputs and sliders to improve usability.
- Use explicit, integer-based column scales (`scale=1` and `scale=2` instead of floating values like `scale=0.5`) to construct standard visual layouts.
