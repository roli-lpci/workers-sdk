---
"miniflare": patch
---

refactor: centralize internal `/cdn-cgi/` paths and move platform proxy endpoint

Internal Miniflare endpoints now use a centralized `CorePaths` constant. The `getPlatformProxy` magic proxy has been moved from the root URL to `/cdn-cgi/platform-proxy`, a reserved path in the Cloudflare Network.
