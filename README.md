# Legal pages (host on GitHub Pages)

Ready-to-host static pages, mirroring your Sleep Architect legal site.

## Host them
1. Put this `legal/` folder's contents in a GitHub Pages repo (e.g. a new
   `readiness-legal` repo, or this repo's `/docs` with Pages enabled).
2. Your URLs become, e.g.:
   - `https://<user>.github.io/readiness-legal/privacy-en.html`
   - `https://<user>.github.io/readiness-legal/terms-en.html`

## Then wire the URLs (3 places)
- `Readiness/Support/LegalLinks.swift` → `privacy` and `terms`
- `AppStore/listing.md` → the two `[Your … URL]` placeholders (en + ru blocks)
- App Store Connect → **App Privacy** (Privacy Policy URL) and **App Information**
  (Privacy Policy + optional Terms / EULA URL)

## Replace these placeholders before publishing
`[EFFECTIVE DATE]` / `[ДАТА]` · `[CONTACT EMAIL]` / `[EMAIL]` ·
`[DEVELOPER / ENTITY NAME]` / `[ИМЯ РАЗРАБОТЧИКА / ЮРЛИЦО]` ·
`[JURISDICTION]` / `[ЮРИСДИКЦИЯ]` · `[YEAR]` / `[ГОД]`

## Notes
- **Privacy Policy** is written to match the app's real v1.0 behaviour
  (everything on-device, no server). It's accurate as-is once you fill the
  placeholders. When v1.1 turns the cloud on, update section 8 / 2.
- **Terms** is a generic starting template — review it (entity, jurisdiction,
  liability) before publishing.
- The Russian pages use formal «вы» (standard for legal text), unlike the app's
  «ты». Say the word if you'd rather they match the app's «ты».
