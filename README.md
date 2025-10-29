# bentleyy — minimal landing page

This is a single-file static site (`index.html`). You can host it anywhere.

## Deploy on Vercel (no Git)
1. Go to https://vercel.com/dashboard
2. Drag `index.html` onto the Projects dashboard to trigger the **Deploy Files** flow.
3. Once deployed, open **Settings → Domains → Add** and attach your domain.
   - `www.bentleyy.com` → CNAME to `cname.vercel-dns.com`
   - `bentleyy.com` (apex) → A record to `76.76.21.21`
4. HTTPS is automatic.

## Deploy on Netlify (drag & drop)
1. Go to Netlify → **Add new site → Deploy manually**.
2. Drag `index.html` in.
3. Add your custom domain in **Site settings → Domain management** and follow their DNS prompts.

## Deploy on cPanel
1. Open **File Manager**, upload `index.html` to `public_html/` (or the subdomain folder).
2. Ensure SSL is enabled (AutoSSL or Let's Encrypt).

## Editing
- The typed line is controlled by the `data-text` attribute inside the `<p class="sub typing">` element.
- Newlines are supported: use either a real newline or `\n` in the attribute.
- Contact link: update the `mailto:` in the `<a class="cta">` if needed.
