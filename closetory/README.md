# Closetory Legal Pages

This directory contains the static pages intended for the public privacy-policy and terms-of-use site:

- `privacy-policy.html`
- `terms-of-use.html`
- `index.html`
- `styles.css`

## GitHub Pages deployment

Copy the four files above into the publishing folder of your prepared GitHub Pages repository. Keep them together: all stylesheet and page links are relative, so they work both at a domain root and under a project-repository path. Do not publish the app source, personal documents, archives, credentials, or signing files.

For example, if your site base is `https://YOUR-USERNAME.github.io/closetory-legal/`, use:

- Privacy URL: `https://YOUR-USERNAME.github.io/closetory-legal/privacy-policy.html`
- Terms URL: `https://YOUR-USERNAME.github.io/closetory-legal/terms-of-use.html`
- Support URL: `https://YOUR-USERNAME.github.io/closetory-legal/`

Replace the example base with the actual URL shown by GitHub Pages; no domain substitution is needed inside these HTML files. `index.html` contains public support contact details.

Before publishing, confirm:

1. The public contact email is correct.
2. The operator/developer identity is accurate: Shurui Chen (陈树锐).
3. The Open-Meteo service description still matches the provider used by the released build.
4. These October 7, 2026 disclosures match the released build, including the 40-item / 20-outfit creation limits, local rule-based recommendations, merge-style imports, and absence of IAP and App-level CloudKit sync.
5. All three pages, language anchors, stylesheet, email links, and links between documents work over HTTPS without login on both Wi-Fi and mobile data in the intended markets. Test the actual deployed URLs, not only local files.
6. The App and App Store Connect point to the deployed privacy URL. Match the App Store privacy questionnaire to actual data handling; do not assume that local-first or no accounts means no information is sent to third parties. Weather requests send system-provided coordinates and an IP address to the provider.
7. The App's weather display also includes appropriate Open-Meteo attribution and a CC BY 4.0 link. Attribution on this website alone is not a substitute for attribution where weather data is displayed. See [Open-Meteo's data license](https://open-meteo.com/en/pricing).
8. Review the provider-selection commitments in the Privacy Policy before publishing. The public provider notices describe safeguards, but they are not an independent audit or a provider-specific contractual confirmation of every App Review requirement. Do not publish claims that you cannot substantiate.
9. Ensure users are informed of the weather recipient and logging before their first weather transmission; a policy URL and a generic system location prompt are not by themselves proof of informed consent to third-party sharing.

## Scope and future updates

These documents describe the current code, not a planned WeatherKit migration. The location accuracy setting is a desired accuracy, not a guarantee of coarse location. Weather snapshots have a 30-minute freshness threshold, not a 30-minute deletion deadline. App-level CloudKit sync is disabled, but Apple system backups may still include local data.

If you add WeatherKit, CloudKit, accounts, analytics, advertising, cloud AI, or in-app purchases, review both pages and the App Store disclosures before shipping. Before monetizing with the current weather provider, separately verify [Open-Meteo's commercial API conditions](https://open-meteo.com/en/terms); being free to download alone does not establish eligibility for its free API.

Publishing these files does not itself add an in-app privacy notice, obtain legally required consent, complete the privacy questionnaire, or establish compliance with every market's laws. Obtain professional legal advice where needed; this is not a guarantee of App Store approval.
