# Palette Journal - SkinGPT-4 UX and Accessibility learnings

## 2025-02-17 - Gradio 3.24.1 UX Patterns
**Learning:** Gradio 3.24.1 lacks `gr.Info`, `gr.Warning`, and `gr.Error` notifications (introduced in 3.33.0+). We must use status updates or parameter configurations to convey hints/warnings cleanly. Wrapping long texts/disclaimers in `gr.Accordion` declutters the UI and focus is kept on interactive elements. Adding descriptive information to inputs (e.g. `label` for `gr.Image`, helper details in labels/sliders) enhances a11y and UX.
**Action:** Always check the installed Gradio version's component support before coding and use status-updates/accordion patterns for version-compatible UX.
