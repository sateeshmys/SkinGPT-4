## 2025-05-15 - Gradio 3.24.1 Compatibility on Python 3.12
**Learning:** Gradio 3.24.1 is incompatible with Python 3.12 for launching servers due to a `TypeError: unhashable type: 'dict'` in Jinja2 templates, and it requires `setuptools<70` because it depends on `pkg_resources`. However, UI components can still be initialized and verified for syntax and parameter validity.
**Action:** Use `python3 -m py_compile` and component initialization (without `.launch()`) for verification in such environments.
