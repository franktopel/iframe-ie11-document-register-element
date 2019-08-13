# IE 11 problem when refreshing an iframe
When document-register-element is loaded in a document which is inside an iframe, refreshing that iframe breaks the polyfill and makes it so `document.createElement` is `undefined`.

## Steps to reproduce

1. Clone the repository
2. npm install
3. npm start
4. Open http://127.0.0.1:8080 in IE 11
5. Open developer tools (F12)
6. Rightclick inside the iframe -> refresh
7. Check console errors.
