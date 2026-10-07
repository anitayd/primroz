# Primroz — Guide Site

Static HTML site for Primroz's pre-launch footwear education hub.

## Structure
- `/` — guide hub
- `/guides/womens-footwear-comfort/`
- `/guides/womens-footwear-fit/`
- `/guides/womens-shoes-materials/`
- `/guides/womens-shoes-durability/`
- `/guides/office-footwear-women/`
- `/guides/styling-womens-footwear/`

## GitHub Pages
1. Create a GitHub repository, e.g. `primroz-site`.
2. Upload all files in this folder to the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)`.
4. GitHub will give you a temporary `github.io` URL.
5. The included `CNAME` file sets the custom domain to `primroz.in`.

## GoDaddy DNS
At GoDaddy DNS, remove conflicting A/AAAA records for the root domain and add GitHub Pages' current apex-domain records as specified by GitHub's Pages documentation. For `www`, create a CNAME pointing to your GitHub Pages hostname. GitHub's current documentation should be treated as authoritative because these IPs can change.

After DNS propagation, add `primroz.in` under **Settings → Pages → Custom domain** and enable HTTPS when GitHub makes it available.

## SEO
The site includes page titles, descriptions, canonical URLs, Open Graph basics, robots.txt and sitemap.xml. Add Google Search Console once the domain resolves and submit `/sitemap.xml`.
