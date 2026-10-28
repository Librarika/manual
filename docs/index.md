# Librarika manual

[Librarika](https://librarika.com) is a cloud-based Integrated Library System (ILS) made by Raynux. Libraries use it in a web browser to manage their catalog, members, loans, holds, fines and reports, and to publish an online public catalog (OPAC). Librarika is hosted at [librarika.com](https://librarika.com), so there is nothing to install.

This manual explains how to use each part of Librarika. Pick the door that fits you:

* **I run a library.** You set up and manage a library: catalog, members, loans and settings. Start with [Getting started](getting-started.md), then see [For library staff](#for-library-staff).
* **I'm a library member.** A library invited you, or you borrow from a library that uses Librarika. Start with the [Member quick start](member-quick-start.md).
* **I use the app or a kiosk.** You use the Librarika app on a phone, as a member or as staff, or a self-checkout kiosk at your library. See [Mobile app and kiosks](#mobile-app-and-kiosks).

## Your Librarika account

You have **one Librarika account**, and it belongs to you, not to a library. With it you can be a member of one library, staff in another, and run a third, all with the same email address and password. You use it on [librarika.com](https://librarika.com), on each library's own website and in the mobile app. How you sign in, your password and two-step verification are set once for the whole account: see [Your account (everyone)](#your-account-everyone).

---

## Overview

* **Who it is for:** school, college and university libraries, public libraries, institutes, organisations, and personal collections.
* **Plans:** a free plan for up to 2,000 copies, and paid plans for larger collections and more features. See [Library settings & plans](libraries.md).
* **Web address:** each library gets its own address, such as `mylibrary.librarika.com`, with its own public catalog.
* **Languages:** the library website can be shown in 21 languages. Some translations are still incomplete.

---

## For library staff

**Setting up**

* [Getting started](getting-started.md): create your library, activate it and invite staff.
* [Library settings & plans](libraries.md): library information, branches, preferences, notifications and plans.
* [Users & roles](users.md): staff accounts, roles and branch access.
* [Members](members.md): members, member groups, invitations and member logins.

**Daily work**

* [Cataloging](cataloging.md): add titles and copies, import and export the catalog.
* [Circulation](circulations.md): check out and check in items.
* [Hold queue](hold-queue.md): holds on items that are checked out.
* [Fees & payments](fees-payments.md): fines, fees and payments.
* [Barcode labels](barcode-labels.md): labels for items and member cards.
* [Reports](reports.md): catalog, circulation, member and purchase reports.
* [Bulk actions](bulk-actions.md) and [Batch update](batch-update.md): change many records at once.

**Sign-in & security for your library**

* [Library sign-in security](library-sign-in-security.md): require two-step verification, set password lengths, ask for new passwords.
* [Single sign-on (SSO with SAML)](sso-saml.md): let people sign in with your organisation's login.
* [Helping people who can't sign in](helping-people-sign-in.md): what to do when a member or colleague is locked out.

**Self-service & kiosks**

* [Self-service](self-service.md): members check items out and in from a browser or phone.
* [SIP2 integration](sip2.md): connect self-checkout kiosks and other SIP2 devices.
* [Kiosk app: setup and management](kiosk-app.md): set up the Librarika Kiosk app on a self-checkout computer.

---

## For members

* [Member quick start](member-quick-start.md): join your library from an invitation, sign in and find your way around.
* [OPAC](opacs.md): the library's online catalog.
* [Member area](member-area.md): what you see when you sign in to your library.
* [Self-service](self-service.md): check items out and in from a browser or phone.
* [Using a kiosk](using-a-kiosk.md): borrow and return at a self-checkout kiosk.

---

## Your account (everyone)

* [Signing in](signing-in.md): password, Google, Apple or your library's SSO.
* [Passwords](passwords.md): the rules, changing your password and resetting a forgotten one.
* [Two-step verification](two-step-verification.md): a code from your phone after your password.
* [Sign-in activity & privacy](sign-in-activity.md): where you are signed in, signing out devices, and what your library can see.

---

## Mobile app and kiosks

The Librarika app for iPhone and Android is for both members and staff; your role in the library you open decides which screens you get.

* [Get the app & sign in](mobile-app.md): install, sign in, choose a library.
* [For members in the app](app-members.md): catalog, loans, holds, self-checkout, balance.
* [For library staff in the app](app-staff.md): scanning, cataloging, cover photos, members, circulation.
* [Account settings in the app](app-account-settings.md): profile, email, password, two-step verification.
* [Troubleshooting the app](app-troubleshooting.md).

At a self-checkout kiosk, members see [Using a kiosk](using-a-kiosk.md); staff set kiosks up with [Kiosk app: setup and management](kiosk-app.md).

[<img class="app-icons ios" src="https://ae85df921b92073b52e8-a126a45a4c59e90797d94cd877fbe744.ssl.cf3.rackcdn.com/static-pages/Download_on_the_App_Store_Badge_US-UK_135x40.svg" alt="Download on the App Store" />](https://itunes.apple.com/us/app/librarika/id1102502605) [<img class="app-icons android" src="https://ae85df921b92073b52e8-a126a45a4c59e90797d94cd877fbe744.ssl.cf3.rackcdn.com/static-pages/google-play-badge.png" alt="Get it on Google Play" />](https://play.google.com/store/apps/details?id=com.librarika.android.dev&hl=en)

---

## Glossary

| Term | Meaning |
|---|---|
| **Librarika account** | Your own sign-in (email address and password), used in every library you belong to, on librarika.com and in the app. |
| **librarika.com (the platform)** | The main Librarika site, where you create an account or a library and see **My Libraries**. Each library also has its own site, such as `mylibrary.librarika.com`. |
| **Member** | Someone who borrows from a library. Some libraries say *patron*. |
| **Staff** | People with a role in a library: library admin, staff (librarian) or assistant. |
| **Library admin** | Staff who manage the library's settings, plan and users. |
| **Two-step verification** | A second step after your password: a 6-digit code from an authenticator app on your phone. |
| **Recovery code** | A one-time code you saved when you turned on two-step verification, for when you don't have your phone. |
| **SSO (single sign-on)** | Signing in to a library with your school's or organisation's own login. |
| **SAML** | The standard Librarika uses to talk to your organisation's sign-in for SSO. |
| **Identity provider (IdP)** | Your organisation's sign-in service that SSO uses, such as Google Workspace or Microsoft Entra ID. |
| **Kiosk** | A self-checkout computer at the library where members borrow and return items. |
| **SIP2 terminal** | A kiosk or other device that connects to Librarika with the SIP2 standard. Each one needs its own licence and terminal account. |

---

## Policies

[Privacy Policy](https://librarika.com/spages/privacy-policy) · [Terms of Use](https://librarika.com/spages/terms-and-conditions-of-use) · [GDPR Statement](https://librarika.com/spages/gdpr-statement) · [Data Processing Agreement](https://librarika.com/spages/customer-gdpr-data-processing-agreement) · [Sub-processors](https://librarika.com/spages/sub-processors)

## Help

Questions? See the [FAQ](faq.md). For questions about your library or plan, [contact us](https://librarika.com/spages/contact). To suggest a correction to this manual, see [Contributing](contribute.md).
