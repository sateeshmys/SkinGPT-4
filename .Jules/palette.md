## 2025-05-22 - Gradio Layout and Component Constraints
**Learning:** Gradio 3.24.1 is extremely sensitive to Python environment versions (3.12+ issues with `pkg_resources`) and layout parameters. `scale` values for `gr.Column` must be integers to avoid warnings, and wrapping long text in `gr.Accordion` significantly improves "above the fold" usability in medical demo applications.
**Action:** Always use integer `scale` for columns (e.g., 1 and 2 for a 1:2 ratio) and use `info` and `label` parameters early to improve accessibility and clarity.
