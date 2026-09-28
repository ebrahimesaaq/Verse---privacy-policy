# Privacy Policy for Versea

**Effective date:** September 28, 2026

Versea ("we," "us," or "our") provides the Versea mobile application (the "App"). This policy explains what information the App handles, how it is used, and the choices available to you.

## Information We Handle

Depending on how you use the App, we and the service providers it relies on may handle:

- **Account information:** email address and password when you create or use an email/password account. Passwords are submitted to Firebase Authentication for account authentication; Versea does not intentionally store passwords in its own Firestore profile documents.
- **Google sign-in information:** when you choose Google sign-in, Google and Firebase Authentication process sign-in credentials and account information made available through that sign-in. Versea uses the signed-in user's display name to populate the profile name when available.
- **Profile information:** the name you enter at registration, or the Google display name, is stored in Firebase Cloud Firestore with an account identifier.
- **Reading progress:** the Bible book, chapter, chapter count, and time of the last reading are stored on your device and, when signed in and connected, synchronized to Firestore under your account identifier.
- **App preferences and saved content:** the App stores reading progress, saved verses, and the verse of the day on your device using local app storage. These local records are not automatically uploaded as a full collection; reading progress is synchronized as described above.
- **Network request information:** the App contacts Google to check internet connectivity and contacts the OurManna service and Bible content API to retrieve app content. Those services may receive standard connection data such as your IP address and request metadata. The app's requests for Bible content include the requested book and chapter identifiers.
- **Notification settings:** the App requests permission to schedule a recurring local Bible reading reminder. The reminder is scheduled on your device; the App code does not send a push notification token to our server.

The App's current dependencies include Firebase Authentication, Cloud Firestore, and Google Sign-In. The project configuration also contains Firebase Analytics identifiers for some platforms, but the app code does not initialize an analytics SDK. Confirm whether analytics or other Firebase products are enabled in the Firebase console or through the final Android build before publishing.

## How We Use Information

We use this information to create and authenticate accounts, display your profile name, save and synchronize your reading progress across sessions, provide requested Bible content and daily verses, and provide the local reading reminder. We may also use information to maintain the security and operation of the App and respond to support requests.

## Service Providers and Sharing

We do not sell personal information. Information is processed by service providers needed to operate the App, including Google Firebase (Authentication and Cloud Firestore), Google (for Google sign-in and connectivity checks), OurManna, and the Bible content API provider. These providers handle information under their own terms and privacy policies. We do not intentionally share profile or reading-progress data with the external Bible content services.

We may disclose information if required by law or where reasonably necessary to protect users, the App, or our legal rights.

## Storage and Retention

Account profile and synchronized reading-progress records are stored in Firebase services. Local preferences and reading-related data remain in app storage on your device until removed by you, cleared by your device, or the App is uninstalled. We retain account and cloud data while needed to provide the service and until it is deleted or no longer needed, subject to applicable legal requirements. **The account and cloud-data deletion process and specific retention period must be confirmed before publication.**

## Your Choices and Requests

You can choose whether to use Google sign-in or an email/password account. You can deny notification permission; this only disables the reminder feature. You may contact us to request access to, correction of, or deletion of account information and associated cloud reading progress. We will need to verify the request and may retain information where the law requires it.

**Account deletion:** Contact us at the email below to request account deletion. Before publishing, the developer should ensure that this request channel is monitored and that deleting an account also removes associated Firestore documents and Firebase Authentication data.

## Children's Privacy

The App is not designed to knowingly collect personal information from children under 13. If you believe a child has provided personal information, contact us so we can review and delete it as appropriate. Confirm the intended age group and applicable local age threshold before publishing.

## Security

We use third-party services and reasonable measures intended to protect information. No internet transmission or electronic storage method can be guaranteed to be completely secure.

## International Processing

Our service providers may process or store information in countries other than the country where you live. The applicable provider terms and settings determine the processing locations.

## Changes to This Policy

We may update this policy as the App or its data practices change. We will publish the updated policy with a revised effective date. Continued use after an update means the updated policy applies to future use, subject to applicable law.

## Contact

**Company:** Verse  
**Email:** [ebrahim.dev10@gamil.com](mailto:ebrahim.dev10@gamil.com)  
**Phone:** 01010977697

## Developer Confirmation Needed Before Google Play Submission

This draft is based on the checked-in Flutter configuration and code. Please confirm or correct these points so the policy and Google Play Data safety answers match actual operations:

1. Is the contact email exactly `ebrahim.dev10@gamil.com` (including the spelling `gamil.com`), or should it be `gmail.com`?
2. Do you use Firebase Analytics, Crashlytics, Google Analytics, advertising SDKs, or any other tracking/diagnostics SDK in the release build or Firebase console? The source has analytics identifiers but no Analytics SDK initialization found in app code.
3. What is your account deletion process, and does it delete Firebase Authentication accounts, Firestore profile documents, and reading-progress documents? What retention period applies to backups or records that cannot be deleted immediately?
4. Is Versea intended for children, or is it directed only to users aged 13 or older (or another local age threshold)?
5. Are there any server functions, admin tools, or other third parties that can access account or reading-progress data beyond Firebase and the named content providers?
6. Please provide the public privacy-policy URL you plan to list in Google Play. This Markdown file can be published on a website or public repository, but a local project file is not itself a public URL.

Update this policy if your answers change any statements above, and make sure the Google Play Data safety form describes the release build and all service-provider practices accurately.
