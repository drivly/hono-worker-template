# Template Cloudflare Worker using Hono with support for HTTP Imports

```javascript
import { Hono } from 'https://pkg.do/hono'
const app = new Hono()

app.get('/', (c) => c.text('Hono!!'))

export default app
```

Uses [drivly/deploy-worker](https://github.com/marketplace/actions/deploy-worker) GitHub Action for 5-10 second deployment times:

```yaml
name: Deploy
on: push
jobs:
  deploy:
    runs-on: ubuntu-latest
    name: Deploy
    steps:
      - uses: actions/checkout@v3
      - uses: drivly/deploy-worker@beta-1
```
