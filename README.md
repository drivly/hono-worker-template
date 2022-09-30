# Template Cloudflare Worker using Hono with support for HTTP Imports

```javascript
import { Hono } from 'https://pkg.do/hono'
const app = new Hono()

app.get('/', (c) => c.text('Hono!!'))

export default app
```
