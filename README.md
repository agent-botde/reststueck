# Reststück Landing Page

Riot Grrrl-inspired landing page for reststueck.de

## Deploy

```bash
vercel deploy --prod
```

## Domain verbinden

Nach dem Deploy:
1. Vercel Dashboard → Project → Settings → Domains
2. `reststueck.de` hinzufügen
3. DNS bei deinem Registrar setzen:
   - A Record: 76.76.21.21
   - CNAME: cname.vercel-dns.com (für www)
