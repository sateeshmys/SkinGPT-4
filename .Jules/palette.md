## 2025-05-15 - Gradio 3.24.1 Compatibility with Python 3.12
**Learning:** Gradio 3.24.1 requires 'pkg_resources' which was removed in setuptools 70+. Additionally, launching a demo on Python 3.12 fails due to Jinja2 template issues with unhashable 'dict' keys in Starlette/FastAPI.
**Action:** Use 'setuptools<70' for installation and rely on 'py_compile' or mock script structural validation instead of full 'demo.launch()' for verification in Python 3.12 environments.
