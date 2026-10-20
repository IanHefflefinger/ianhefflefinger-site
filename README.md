# ianhefflefinger.com

Static personal site: `index.html`, `style.css`, `404.html`, and `assets/`. No build step and no dependencies.

Preview locally: `python3 -m http.server 8000`, then open http://localhost:8000

Deploys automatically on every push to `main` via GitHub Actions (OIDC, no stored AWS keys): sync to S3, then CloudFront invalidation.
