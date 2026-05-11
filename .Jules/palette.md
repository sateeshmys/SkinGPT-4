## 2025-05-14 - Gradio 3.24.1 Compatibility and Layout Constraints
**Learning:** Gradio 3.24.1 requires integer `scale` values for `gr.Column` to avoid layout warnings and potential rendering issues. Additionally, this version has a hard dependency on `pkg_resources` which causes launch failures in Python 3.12 environments.
**Action:** Use integer values for component scales (e.g., 1 and 2 instead of 0.5). Rely on static analysis (`py_compile`) for verification when runtime execution is blocked by environment incompatibilities.
