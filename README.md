# pyEditor.js

A very simple [Editor.js](https://editorjs.io) parser written in pure Python.

Soon-to-be published on [PyPI](https://pypi.org).

## Update:

Currently unmaintained, I'll look at this somewhere during summer 2022, if I'll have time.

### Features:
- Automatically convert Editor.js's JSON output to HTML;
- Sanitization and automatic anchor link converting done by using [bleach]();
- Supports Tailwind CSS by default;
- WYSIWYG - output is made to look as similar to editor as possible.


### Basic Usage:

pyEditorJS requires Python 3.6 or newer. It is very simple to get started:

```python
from pyeditorjs import load

DATA = ... # JSON string/dict of Editor.js output data
HTML = load(DATA)

print(HTML) # HTML str
```

You can then pass the HTML string to a parser like [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) to beautify or modify the result HTML.

See `example.json` => `example.html` files in [this project's GitHub repository](https://github.com/CWKevo/pyeditorjs) for sample outputs.


### TO-DO:
1. Add support for all out-of-box Editor.js elements;
2. Do a PyPI release (using GH actions);
3. Add support for more blocks from Editor.js extensions


## 🎁 Support me

I create free software to benefit people.
If this project helps you and you like it, consider supporting me by donating via [PayPal](https://www.paypal.com/donate/?hosted_button_id=XDUWS5K6947HY).
