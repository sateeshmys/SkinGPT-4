## 2025-05-14 - Gradio 3.24.1 Compatibility and UX Patterns

**Learning:** Gradio 3.24.1 requires `setuptools < 70` to avoid missing `pkg_resources` on Python 3.12. Furthermore, `demo.launch()` fails on Python 3.12 due to a `TypeError: unhashable type: 'dict'` in Jinja2 templates when rendering the interface. However, the UI components themselves can still be initialized and validated via static analysis (`py_compile`).

**Action:** Use `python3 -m py_compile` for verification when a full launch is impossible. When improving the UI, leverage `gr.Accordion` for long text like disclaimers and use the `info` parameter on sliders to explain technical impact, as these are supported in 3.24.1.

**Learning:** Explicit labels for `gr.Image` are crucial for screen reader accessibility and user clarity, especially in medical/diagnostic contexts.

**Action:** Always provide the `label` parameter to `gr.Image` components.
