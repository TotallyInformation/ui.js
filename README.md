# ui.js
A small but powerful library for both the browser and node.js that takes standardised JSON input and converts to HTML.

Originally written to support the `uibuilder` package for Node-RED, this is now made available as a standalone library for use in any project.

It rationalises the MANY quirks and inconsistencies of DOM handling but still stays close to standard HTML terminology so that learning the simple configuration data style used by the library will also help build better HTML knowledge and skills should you desire it. However, only a minimal understanding of HTML is needed.

Distribution versions are provided both for the browser (in both IIFE and ESM formats) and for Node.js (in both CommonJS and ESM formats).

To facilitate the Node.js builds, the `window` object must be passed to the class on instantiation. For Node.js, the `window` object must be provided by loading the [`jsdom`](https://github.com/jsdom/jsdom) library.

Two other optional functions may be passed to the class. One for custom logging and the other for doing syntax highlighting of JSON. If not provided, dummy functions are used that produce no output.
