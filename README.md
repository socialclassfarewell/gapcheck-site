# gapcheck-site

Landing page for **gapcheck.net** (apex 301s to www.gapcheck.net).

Copy must pass caravan-co marketing_qa + engine affiliation/urgency gates before
any deploy (verified 2026-07-21).

**Deploy: GitHub Pages** from this repo, custom domain via `CNAME`. DNS is at
GoDaddy (`ns05/ns06.domaincontrol.com`); A records point at GitHub Pages
(185.199.108–111.153), `www` CNAMEs to `socialclassfarewell.github.io`. Mail is
Zoho Australia — do not change the MX or SPF records when touching site DNS.
See ledger-foundry `docs/specs/gapcheck-dns.md` for the full sheet.

## Copy rules

- **No "audit-readiness" framing.** Dropped deliberately (ledger-foundry `5ea962d`).
  We do not claim to make anyone audit-ready and make no outcome claims.
- **Data handling must match the privacy policy**, which discloses overseas
  processing and AI-assisted document review. The site previously claimed
  "Documents stay in Australia. No external AI upload" — that contradicted the
  privacy policy and offer.txt, and was corrected 2026-08-28.
- **Opt-out wording must match live outreach.** Outreach says "unsubscribe";
  the site honours both that and "stop".
