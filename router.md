## Static-file server improvements

v1.x implementation

`assets` path is fixed. All resources should be added to this directory.

v2.x implementation

Similar to any other static server, url path will represent the file path on disk.

Eg:

- `http://localhost:5000/app.js` will load `./app.js`
- `http://localhost:5000/resources/home.png` will load `./resources/home.png`
- Both `http://localhost:5000/` and `http://localhost:5000` (without ending `/`) will load `./index.html`


## Native interface protocol

v1.x implementation

Uses `POST/GET http://localhost:5000/<module>/<method>`

v2.x implementation

Will use `POST/GET http://localhost:5000/__nativeMethod_<module>.<method>`. So there is no confusion with file paths.
