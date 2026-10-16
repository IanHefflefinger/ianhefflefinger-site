# ianhefflefinger.com

Static personal site. No build step and no dependencies: `index.html`, `style.css`, and `assets/`.

Preview locally: `python3 -m http.server 8000` inside this folder, then open http://localhost:8000

Deploy by hand (until automated):
`aws s3 sync . s3://YOUR-BUCKET --exclude ".git/*" --exclude "README.md"`
then `aws cloudfront create-invalidation --distribution-id YOUR-ID --paths "/*"`
