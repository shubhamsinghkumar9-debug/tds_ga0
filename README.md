# eShopCo latency metrics API

## Endpoint
After deployment, POST to `https://YOUR-VERCEL-DOMAIN.vercel.app/api/metrics`.

## Deploy
1. Create a new GitHub repository and push these project files.
2. Import the repository at https://vercel.com/new.
3. Deploy with the default settings.
4. Test the deployed endpoint:

```bash
curl -X POST 'https://YOUR-VERCEL-DOMAIN.vercel.app/api/metrics' \
  -H 'Content-Type: application/json' \
  -d '{"regions":["apac","amer"],"threshold_ms":182}'
```

The response contains `avg_latency`, `p95_latency`, `avg_uptime`, and `breaches` for each requested region. CORS allows any origin for POST and OPTIONS requests.
# project
