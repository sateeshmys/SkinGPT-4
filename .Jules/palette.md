# Palette's Journal - Critical Learnings Only

## 2025-02-12 - Explicit Accessible Labels for Image Upload Components in Gradio 3.24.1
**Learning:** In Gradio 3.24.1, `gr.Image` components default to no label or accessibility attributes if the `label` parameter is omitted. Providing an explicit label parameter (e.g. `label="Upload Skin Image"`) not only makes the UI visually clearer but also significantly improves screen-reader accessibility by offering a descriptive text label.
**Action:** Always provide explicit, user-friendly `label` attributes for any image upload or interactive elements in Gradio to ensure visual clarity and accessibility conformance.
