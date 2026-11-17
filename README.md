# Digiiplex legal pages

Static HTML for GitHub Pages. No build, JavaScript, database, API keys, or third-party font assets are required. The existing kaifott files remain separate in D:\digiiplex-org\privacy-policy. These Digiiplex pages are now located in D:\digiiplex-org\digiiplex-privacy-policy.

## Files and publication URLs

The original kaifott repository remote is `https://github.com/kaifali744/kaifott-privacy-policy.git`.
If you copy these pages into a digiiplex subfolder of that original repository and publish its root, these will be the URLs **after you push and Pages finishes deploying**. For a separate repository, follow the new-repository instructions below; these old-repository URLs will not apply automatically:

| Purpose | File | Expected URL |
| --- | --- | --- |
| Legal overview | `digiiplex/index.html` | https://kaifali744.github.io/kaifott-privacy-policy/digiiplex/ |
| Play Console privacy policy | `digiiplex/privacy-policy.html` | https://kaifali744.github.io/kaifott-privacy-policy/digiiplex/privacy-policy.html |
| Play Console account deletion | `digiiplex/account-deletion.html` | https://kaifali744.github.io/kaifott-privacy-policy/digiiplex/account-deletion.html |
| App trader Terms of Service | `digiiplex/terms-of-service.html` | https://kaifali744.github.io/kaifott-privacy-policy/digiiplex/terms-of-service.html |

These addresses are inferred from the Git remote, not a verified deployment. If you use a different repository, a custom domain, or publish this folder as the repository root, use the Pages URL shown by GitHub and append the corresponding filenames. The links between pages are relative and continue to work at a repository root or subfolder.

## Business address and phone

The public details supplied by the owner are included in `terms-of-service.html`, inside `<section id="business-contact">`:

INNOV8 PRESTIGE TECH PLATINA,
11th FLOOR, NO.32/2,34/1, VARTUR,
BANGALORE SOUTH, BANGALORE-560087.

Phone: +91 8123317555 (clickable telephone link).

For future changes, edit that section. The privacy policy links to it, so the address can be maintained in one place. Use matching details in your Play Console trader profile. The confirmed legal operator and monitored email are Digiiplex Entertainment Pvt Ltd and support@digiiplex.com.

## Optional: publish using the existing kaifott repository

1. Review the business contact details above and the operating commitments below.
2. Copy the contents of `D:\digiiplex-org\digiiplex-privacy-policy` into a `digiiplex` subfolder of `D:\digiiplex-org\privacy-policy`. Add and commit that subfolder, then push it to the branch already used by GitHub Pages.
3. In the GitHub repository's **Settings > Pages**, confirm the source. For branch publishing, use the intended branch and `/(root)`. This preserves the old kaifott URLs and publishes the new subfolder. GitHub cannot select an arbitrary `/digiiplex` folder as the source for branch publishing; it must be inside the published root (or copied into a supported source).
4. Wait for the Pages deployment to succeed. Open all three policy URLs while signed out, including on mobile. They must load publicly over HTTPS without login or geographic restrictions.
5. Enter the privacy URL and deletion URL in the respective Digiiplex app fields in Play Console / Data safety. Enter the terms URL in that app's trader-status / Terms of Service declaration.
6. Complete the account-level trader declaration, app-level confirmation, verified business contact details, and required self-certification separately in Play Console.
7. Keep the in-app policies and disclosures consistent with these pages and with the Data safety form.

If making a **new repository**, copy the contents of this folder into its root and enable Pages from that root. The URLs will then be `https://YOUR-OWNER.github.io/YOUR-REPOSITORY/privacy-policy.html`, `account-deletion.html`, and `terms-of-service.html`. No hosting manifest or Sites deployment is needed.

## Operating details to check before official submission

- **Email workflow:** The prominent deletion button opens an email draft; it does not submit a form or automatically delete an account. The monitored mailbox must actually receive, verify, process, and confirm requests. Test delivery yourself. Provide the requester an expected completion time; no arbitrary 7/30/90-day promise has been invented.
- **Retention:** At the owner's request, the pages omit unestablished numeric backup/payment retention periods. They retain a general explanation of payment/legal/security exceptions and backups. This is not a verified retention schedule. Establish applicable periods with the people responsible for payments, backups, and legal record keeping; update both the privacy and deletion pages when known. Do not promise that every record disappears immediately.
- **Deletion coverage:** The reviewed auth service clears account fields, deletes profiles and device sessions, invalidates sessions, and retains a deleted-account record linked to payments. This is not proof that all account-linked information is erased across services. The analytics schema has user/profile-linked playback and watch-history records, and the inspected deletion handler does not explicitly purge those records or request deletion from external providers. Verify database cascades/triggers and cross-service/provider cleanup with the deployed backend. Include any remaining associated data in the support deletion workflow unless a justified, disclosed retention exception applies.
- **Existing Android terms differ:** Mobile `app/src/main/java/com/digiiplex/ui/profile/sections/StaticContentScreen.kt` and TV `tv/src/main/assets/terms.txt` still say all premium memberships recur and contain a blanket partial-month no-refund statement. The new web terms distinguish prepaid and auto-renewing offers and preserve mandatory consumer rights. Synchronize the Android terms or link to the published terms before release. Android files have not been changed by this task.
- **Privacy consistency:** The starting point was the app's November 12, 2026 privacy asset, checked against app features. Confirm the final release's SDK configuration and actual backend handling match the disclosures, especially location for advertising, IP-based lookup, Google IMA, Crashlytics, Facebook sign-in, payments, and messaging.
- **Children and consent:** The current app uses DOB for Kids profiles and does not enforce a minimum age. Neither a Kids profile nor a legal page proves parental consent or compliance with children's requirements. Confirm target-audience declarations, permissions, and any required consent in the released app.
- **Payments:** The terms describe purchase options; they do not establish that every payment option is permitted in every Play market or program. Use the payment flow applicable to your actual release.
- **App/operator names:** Keep “Digiiplex” and “Digiiplex Entertainment Pvt Ltd” consistent with your official listing. If either changes, update every page.
- **Dates:** Update the effective/last-updated dates when you approve later changes.
- These files provide public documents and a deletion request route. They do not implement backend deletion, prove mailbox delivery, complete trader verification, or guarantee Play approval.

## Verification and maintenance

Open `index.html` locally to preview; relative navigation and styles work without a server. The pages include semantic headings, keyboard focus styles, a skip link, responsive layouts, and print styling. No cookies, analytics scripts, or account-input form are added by these files. The hosting provider and email provider still process their normal request/message information.

For optional local HTTP preview from this folder, run `python -m http.server 8000 --bind 127.0.0.1` and open `http://127.0.0.1:8000/`. Stop it with Ctrl+C when finished.

The `.nojekyll` file is useful when publishing this folder's contents as a new repository root. In the existing repository it does not change root-level Jekyll settings; plain HTML/CSS needs no Jekyll features.

## Official references reviewed on 17 November 2026

- [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311?hl=en)
- [Google Play account deletion requirements](https://support.google.com/googleplay/android-developer/answer/13327111?hl=en)
- [Google Play trader status declaration](https://support.google.com/googleplay/android-developer/answer/17594752?hl=en)
- [GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
