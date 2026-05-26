## 2025-05-14 - Gradio 3.24.1 Layout and Info Patterns
**Learning:** Gradio 3.24.1 supports 'info' and 'label' parameters for form components, which are essential for explaining complex AI parameters (like Temperature/Beam Search) to users. It also supports 'gr.Accordion' for managing long secondary content. However, the 'scale' parameter in 'gr.Column' is more reliable when using integer values (e.g., 1:2 ratio) rather than decimals in this version.
**Action:** Always use 'info' text to clarify AI-specific settings and stick to integer 'scale' values for robust layout control in older Gradio versions.

## 2025-05-14 - Python 3.12 and Gradio 3.24.1 Compatibility
**Learning:** Gradio 3.24.1 is incompatible with Python 3.12 for server launching due to a Jinja2 template error ('TypeError: unhashable type: dict'). Additionally, it requires 'setuptools<70' because 'pkg_resources' was removed in newer versions.
**Action:** Use 'python3 -m py_compile' for syntax verification when the environment prevents actual launching, and ensure 'setuptools<70' is installed for environment setup.
