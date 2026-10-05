# sangojpn-brand-assets

Public brand logos and per-article Open Graph PNGs for [sangojpn.com](https://www.sangojpn.com/).

**Why public?** The main pipeline repo `sangojpnet/ai-tech-brief` is private. Blogger / social
thumbnails need HTTPS URLs that work without GitHub auth. This repo holds only logos and
generated OG images — no secrets, no source code.

## Public URLs

- Logo (header / fallback):  
  `https://raw.githubusercontent.com/sangojpnet/sangojpn-brand-assets/main/brand/logo-horizontal-white-2000.png`
- Per-article OG:  
  `https://raw.githubusercontent.com/sangojpnet/sangojpn-brand-assets/main/og/<name>.png`

Optional CDN mirror (jsDelivr):  
`https://cdn.jsdelivr.net/gh/sangojpnet/sangojpn-brand-assets@main/brand/logo-horizontal-white-2000.png`

## Layout

```
brand/   # static Sangojpn logos
og/      # generated 1200×630 PNGs (AI & Tech Brief, X repost digest, …)
```

Uploads are done by the private `ai-tech-brief` pipeline via the GitHub Contents API
(using a fine-grained PAT scoped to this repo). Do not put API keys or OAuth tokens here.
