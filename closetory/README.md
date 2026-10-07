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
3. The WeatherKit / Apple Weather service description matches the released build; no alternate weather provider is used.
4. These October 7, 2026 disclosures match the released build, including the 40-item / 20-outfit creation limits, local rule-based recommendations, merge-style imports, and absence of IAP and App-level CloudKit sync.
5. All three pages, language anchors, stylesheet, email links, and links between documents work over HTTPS without login on both Wi-Fi and mobile data in the intended markets. Test the actual deployed URLs, not only local files.
6. The App and App Store Connect point to the deployed privacy URL. Match the privacy questionnaire to actual data handling; WeatherKit alone does not establish “Data Not Collected.” Queries send coordinates rounded to two decimal places; network connections involve IP information.
7. Both weather displays use official Apple Weather marks and the legal URL returned by WeatherService.attribution. Website attribution alone is insufficient. See [Apple's requirements](https://developer.apple.com/weatherkit/).
8. Review the provider-selection commitments in the Privacy Policy before publishing. The public provider notices describe safeguards, but they are not an independent audit or a provider-specific contractual confirmation of every App Review requirement. Do not publish claims that you cannot substantiate.
9. Confirm versioned, explicit weather opt-in and withdrawal work before sending coordinates. A policy URL and a generic location prompt alone do not establish informed consent.
10. Enable WeatherKit under both Capabilities and App Services for com.RexChan.Closetory in the developer portal, refresh signing profiles, and test a signed build on a device. Local entitlement configuration and simulator tests do not establish service authorization.

## Scope and future updates

These documents describe the native WeatherKit implementation. The App rounds coordinates explicitly before transmission; desiredAccuracy alone is not the privacy safeguard. Snapshot usability ends at the earlier of 30 minutes and Apple's expiry; expired cache is removed on next access or launch, not by a promised background deletion timer. App-level CloudKit sync is disabled, but system backups may still include local data. No server-log retention period or processing region is guaranteed by these pages.

If you add CloudKit, accounts, analytics, advertising, cloud AI, or in-app purchases, review both pages and App Store disclosures before shipping. Review Apple WeatherKit quotas, attribution, cache limits, and applicable developer agreements before monetization. Do not silently introduce another provider.

Publishing these files does not itself add an in-app privacy notice, obtain legally required consent, complete the privacy questionnaire, or establish compliance with every market's laws. Obtain professional legal advice where needed; this is not a guarantee of App Store approval.
