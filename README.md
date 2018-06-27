# SystemJS HMR

Hack the original [systemjs-hmr](https://github.com/alexisvincent/systemjs-hmr) to support SystemJS >= 20.

Meant to override [systemjs-hot-reloader]()'s dependency. For instance with JSPM:

```json
{
  "jspm": {
    "overrides": {
      "npm:systemjs-hot-reloader@1.1.0": {
        "dependencies": {
          "systemjs-hmr": "github:KoltesDigital/systemjs-hmr"
        },
        "map": {
          "./dist/index.js": {
          "production": "./lib/production.js"
          }
        }
      }
    }
  }
}
```
