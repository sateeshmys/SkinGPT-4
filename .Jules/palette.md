## 2025-05-14 - Gradio 3.24.1 and Python 3.12 Compatibility
**Learning:** Gradio 3.24.1 requires 'pkg_resources', which is removed in setuptools 70+. Additionally, 'demo.launch()' fails on Python 3.12 with a 'TypeError: unhashable type: dict' in Jinja2 templates.
**Action:** Use 'pip install "setuptools<70"' to fix 'pkg_resources' issues. For UI verification on Python 3.12, rely on 'py_compile' and static analysis or mock scripts (without .launch()) since the server cannot start.
