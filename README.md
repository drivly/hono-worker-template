# hono-worker-template
Template Cloudflare Worker using HonoJS with HTTP Imports

```javascript
import { Hono } from 'https://pkg.do/hono'
const app = new Hono()

app.get('/', (c) => c.text('Hono!!'))

export default app
```
