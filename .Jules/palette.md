## 2026-04-20 - Gradio 3.24.1 Environment Constraints
**Learning:** Gradio 3.24.1 relies on deprecated modules (distutils, pkg_resources) and is incompatible with Python 3.12+. Attempting to run it in newer environments results in ModuleNotFoundErrors.
**Action:** Always verify environment compatibility before attempting local UI execution. Use 'py_compile' for basic code validation when full environment setup is not feasible.

## 2026-04-20 - Gradio Layout Precision
**Learning:** In Gradio 3.24.1, 'scale' values for layout components like 'gr.Column' should be integers. Using floats (e.g., 0.5) can trigger UserWarnings and inconsistent layout behavior.
**Action:** Ensure all layout scale parameters are integers for this version of Gradio.
