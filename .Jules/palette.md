## 2025-06-25 - Gradio 3.24.1 UX Patterns for Medical AI

**Learning:** In medical AI applications, transparency and interface focus are critical. Parameter sliders (like Beam Search and Temperature) often confuse non-expert users without explanatory text. Additionally, long legal/medical disclaimers can push active interactive elements "below the fold," degrading the user experience.

**Action:**
1. Use the 'info' parameter in Gradio components to provide contextual help for technical settings.
2. Encapsulate secondary but mandatory text (like disclaimers) in 'gr.Accordion' to maintain layout focus.
3. Use integer values for 'scale' in 'gr.Column' to ensure reliable layout ratios (e.g., 1:2 instead of 0.5:1).
4. Apply 'variant="secondary"' to reset/clear actions to establish a clear visual hierarchy against the primary 'Submit' or 'Upload' actions.
