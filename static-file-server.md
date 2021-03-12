## Flexible static-file server improvements

v1.x implementation

`assets` path is fixed. All resources should be added to this directory.

v2.x implementation

Similar to any other static server, url path will represent the file path on disk.

Eg:

- `http://localhost:5000/app.js` will load `./app.js`
- `http://localhost:5000/resources/home.png` will load `./resources/home.png`
- `http://localhost:5000/` will load `./index.html`
