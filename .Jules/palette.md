## 2025-05-14 - Gradio 3.24.1 Layout Constraints
**Learning:** Gradio 3.24.1 requires integer values for the `scale` parameter in layout components like `gr.Column`. Using floats (e.g., 0.5) triggers a UserWarning and can cause inconsistent layout behavior.
**Action:** Use integer scales to define proportions (e.g., use `scale=1` and `scale=2` instead of `scale=0.5` and `scale=1.0`) to maintain desired ratios without triggering warnings.

## 2025-05-14 - Decluttering Medical Interfaces
**Learning:** Medical AI interfaces often include long disclaimers and complex parameters that can push the primary interaction (e.g., image upload) below the fold.
**Action:** Use `gr.Accordion` (closed by default) for secondary content like disclaimers and use the `info` parameter in sliders to provide context without overcrowding the label.
