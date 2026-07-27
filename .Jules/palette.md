# Palette's UX & Accessibility Journal

## 2025-02-14 - [Collapsible Medical Disclaimers]
**Learning:** Medical disclaimers, while extremely important for safety and liability, can consume excessive visual real estate in AI medical diagnostics. Collapsing them into a `gr.Accordion` defaulting to `open=False` and removing redundant headers keeps user focus on the main tool and primary interactive functions.
**Action:** Always group lengthy, legal, or non-actionable texts into a default-collapsed accordion container.

## 2025-02-14 - [Integer-Based Column Scaling in Gradio 3.24.1]
**Learning:** Gradio 3.24.1 works best with integer scaling factors (such as `scale=1` and `scale=2`) rather than floats (e.g., `scale=0.5`). Setting clean, relative integer scales guarantees a robust 1:2 layout across different screen sizes.
**Action:** Use integer weights for relative column layouts to avoid visual distortions.

## 2025-02-14 - [Descriptive Parameters with Slider Info fields]
**Learning:** High-level sliders in AI models (like "Temperature" or "Beam Search Numbers") can be confusing to lay users or clinical staff. Adding a clear `info` parameter to explain the underlying implications (such as diagnostic diversity or processing latency) demystifies model configuration parameters.
**Action:** Always provide descriptive `info` text detailing technical trade-offs on Gradio slider components.

## 2025-02-14 - [Visual Button Hierarchy & Screen Reader Accessibility]
**Learning:** Placing secondary buttons (like 'Restart' or 'Clear') with primary styling can distract users from the key call to action ('Upload'). Furthermore, omitting explicit labels on `gr.Image` components leaves screen readers without proper context.
**Action:** Style secondary buttons with `variant="secondary"` and explicitly set clear `label` fields on `gr.Image` for robust screen reader access.
