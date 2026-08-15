# mafft-websockex

Pull the main article text out of a news or blog page, stripping nav, ads, and boilerplate.

```javascript
const extract = require("mafft-websockex");

const dom = new JSDOM("...");
const { html, text } = extract(dom.window.document.body);
```

Returns both the cleaned HTML fragment and the plain text.
