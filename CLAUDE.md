# CLAUDE.md — spirelead

Landing page for **spirelead.co**, a cold-email sending domain bought through Zapmail and used by project arb's
drew@/sloane@/brett@ inboxes. One static page: "Spirelead, a Dharma Loop company", links to dharmaloop.com
(Ink design copied from ~/Code/dharmaloop), `noindex`. This repo is PUBLIC on purpose (free GitHub Pages): never
put anything non-public here.

## Hosting
- GitHub Pages from `main` (root), custom domain via `CNAME`, HTTPS enforced. Push to `main` = deploy.
- DNS stays at Zapmail (domain registered by Zapmail at Namecheap, nameservers Google Cloud DNS, edited in the
  Zapmail app > Domains > spirelead.co > DNS Records): apex A records = GitHub Pages IPs (185.199.108-111.153),
  `www` CNAME `ques123.github.io`. Zapmail's own domain forwarding is OFF. Never touch the MX/SPF/DKIM/DMARC records.
- Why not babbage: babbage's firewall only accepts Cloudflare, and the domain cannot move to Cloudflare (Zapmail owns
  the registrar account).
