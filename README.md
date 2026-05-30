# sutradb.org redirect

Static GitHub Pages site that redirects **sutradb.org** → <https://loka.emmaleonhart.com/>.

The previous DNS/URL-forwarding setup had no valid HTTPS certificate, so
`https://sutradb.org` failed the TLS handshake. GitHub Pages issues a free
Let's Encrypt certificate for the custom domain, fixing HTTPS.

## DNS setup (to do at the registrar)
Point `sutradb.org` at GitHub Pages with these apex A records:
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

The `CNAME` file in this repo sets the Pages custom domain to `sutradb.org`.
