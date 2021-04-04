## Renaming

v1.x implementation

File path: `app/settings.json`

v2.x implementation

File path: `./neutralino.config.json`

## Structure

v1.x implementation

```js
{
  "appname": "test-app",
  "appport": 8080,
  "mode": "window",
  "url": "/",
  "globals": {
    "TEST": "value"
  },
  "window": {
    "title": "Test app",
    "fullscreen": false,
    "alwaysontop": false,
    "iconfile": "app/test-icon.png",
    "borderless": false,
    "maximize": false,
    "width": 800,
    "height": 600,
    "enableinspector": false
  },
  "cloud": {
    "blacklist": [ "os.runCommand" ]
  },
}
```

v2.x implementation

```js
{
  "applicationId": "js.neutralino.testApp",
  "port": 8080,
  "defaultMode": "window",
  "url": "/app", // Eg: /index.html, /app/home.html, https://neutralino.js.org
  "globalVariables": {
    "TEST": "value",
    "NUM": 500
  },
  "nativeBlockList": ["os.*", "debug.log"],
  "modes": {
    "window": {
      "port": 5006,
      "title": "Test app",
      "fullScreen": false,
      "alwaysOnTop": false,
      "icon": "app/test-icon.png",
      "borderless": false,
      "maximize": false,
      "width": 800,
      "height": 600,
      "enableInspector": false
    },
    "cloud": {
    },
    "browser": {
    }
  }
}
```
