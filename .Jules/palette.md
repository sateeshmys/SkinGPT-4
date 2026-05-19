## 2024-05-22 - Gradio 3.24.1 Compatibility with Python 3.12
**Learning:** Gradio 3.24.1 requires `pkg_resources`, which was removed in `setuptools` version 70+. In Python 3.12+ environments, this causes `ModuleNotFoundError: No module named 'pkg_resources'`. Additionally, while components can be initialized, `demo.launch()` fails with `TypeError: unhashable type: 'dict'` due to Jinja2 template issues in this specific Gradio version when running on Python 3.12.
**Action:** Use `pip install "setuptools<70"` to fix the import error. For UI verification, rely on `py_compile` and mock scripts that initialize layout without calling `.launch()` if the environment prevents server execution.

## 2024-05-22 - Medical AI UX Patterns
**Learning:** Medical AI applications often have dense disclaimers and technical parameters (Temperature, Beam Search) that clutter the UI and confuse non-technical users.
**Action:** Wrap long disclaimers in `gr.Accordion(open=False)` to maintain focus on core interactions. Use the `info` parameter in `gr.Slider` to provide inline explanations of how parameters affect diagnostic quality and latency. Always use explicit `label` on `gr.Image` for accessibility.
