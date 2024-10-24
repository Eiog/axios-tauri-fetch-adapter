# axios-tauri-fetch-adapter

[![](https://img.shields.io/npm/v/axios-tauri-fetch-adapter)](https://www.npmjs.com/package/axios-tauri-fetch-adapter)
[![](https://img.shields.io/npm/l/axios-tauri-fetch-adapter)](https://github.com/Eiog/axios-tauri-fetch-adapter/blob/main/LICENSE)

Makes it easy to use Axios in Tauri App, Adapted for Tauri App 2.0.0

# Installation

```
npm install axios-tauri-fetch-adapter
```

# Usage

###  **TypeScript / JavaScript**

```js
import axios from 'axios'
import axiosTauriApiAdapter from 'axios-tauri-fetch-adapter'
const client = axios.create({ adapter: axiosTauriFetchAdapter })
```

### **Tauri App**

Configure the allowed URLs [Tauri App HTTP client](https://v2.tauri.app/plugin/http-client/#usage)

```json5
{
  "permissions": [
    {
      "identifier": "http:default",
      "allow": [{ "url": "https://*.tauri.app" }],
      "deny": [{ "url": "https://private.tauri.app" }]
    }
  ]
}
```

# License

MIT
