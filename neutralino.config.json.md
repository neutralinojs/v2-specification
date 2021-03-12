## Renaming

v1.x implementation

File path: `app/settings.json`

v2.x implementation

File path: `./neutralino.config.json`

## Structure

v1.x implementation

```json
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

```json
{
  "applicationId": "js.neutralino.testApp",
  "port": 8080,
  "defaultMode": "window",
  "entryPath": "/", // Eg: /index.html, /assets/home.html
  "globalVariables": {
    "TEST": "value",
    "NUM": 500
  },
  "blockList": ["os.*", "debug.log"],
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
      "enableinspector": false,
      "globalVariables": {
        "TEST": "value",
        "NUM": 500
      }
    },
    "cloud": {
      "port": 5016,
      "globalVariables": {
        "TEST": "value",
        "NUM": 500
      }
    },
    "browser": {
      "port": 5026,
      "globalVariables": {
        "TEST": "value",
        "NUM": 500
      }
    }
  }
}
```
