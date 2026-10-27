# Sign-in & Security

This page explains the different ways to sign in to Librarika, how to see where your account is signed in, and how to sign out of a device you don't recognise. It is written for everyone: library staff, members and people who only use the mobile app.

Your **Librarika account** belongs to you, not to one library. You use the same account on [librarika.com](https://librarika.com), in every library you belong to and in the mobile app.

---

## Ways to sign in

On a library's login page (and on librarika.com) you can sign in with:

* **Username (email) and password** -- your Librarika password.
* **Google** -- the Google account that uses the same email address as your Librarika account.
* **Apple** -- your Apple ID, if it uses the same email address as your Librarika account.
* **SSO** (single sign-on, the key icon) -- your school's or organisation's own login. This button only appears in libraries that have [SSO](sso-saml.md) switched on.

![Library login page with SSO, Google and Apple buttons](img/signin-library-login-buttons.png)

On [librarika.com](https://librarika.com) the buttons read **Sign in with Google** and **Sign in with Apple**:

![Librarika.com login page with Google and Apple buttons](img/signin-librarika-login-buttons.png)

**Good to know:**

* Google and Apple sign you in to an **existing** Librarika account with the **same email address**. They don't create a new account. If no account uses that email, you will see *"No user account is associated with the connected Google account. Please register a new account."*
* Your account must be verified first. A new account that hasn't confirmed its email yet is asked to *"verify your email address in order to login."*
* Apple's **Hide My Email** option gives Librarika a private relay address (ending in `privaterelay.appleid.com`), which won't match your Librarika email. Choose **Share My Email** when Apple asks, or sign in with your password.

### Signing in with your organisation's SSO

If your library uses SSO, click the key icon on the library's login page and sign in on your organisation's page. You come back to the library already signed in.

* Your organisation's SSO can only sign you in to libraries that are **ticked in your own [SSO sign-in list](#your-sign-in-settings)**. The library is ticked for you when its SSO created your account.
* Some libraries allow **SSO only**. On their website, a sign-in with a password, Google or from *My Libraries* on librarika.com is not accepted there; you will see *"This library allows sign-in with its SSO only. Please sign in with SSO."* Your account still works everywhere else.

### Your Librarika password and your organisation's password

When you accept an invitation from a library, you create a **new password for Librarika**. It is separate from your email account's password and from your organisation's SSO password, so don't reuse those. You need it on librarika.com and in other libraries you join, where your organisation's SSO can't sign you in.

---

## Your sign-in settings

Open your settings: members click `My Account` > `Account Settings`; staff click the settings menu (gear icon) at the top right > `Settings`.

![SSO sign-in list and the Google sign-in switch in Account Settings](img/signin-member-settings-sso-google.png)

* **SSO sign-in** -- the libraries whose SSO may sign you in. Untick a library to stop its SSO from signing in to your account. This list only appears if you belong to a library that uses SSO.
* **Enable Google Login** and **Sign in with Apple** -- your own switches for Google and Apple.
* Click `Save Settings` when you are done.

If you signed in **with SSO**, you can look at these settings but not change them. You will see *"You signed in with SSO. Sign in with your password or Google to …"*. This protects your account: whoever controls an SSO login can't change how your account signs in.

---

## Sign-in activity

At the bottom of **Account Settings** you will find **Sign-in activity**. It shows where your account is signed in and every sign-in of the last 90 days.

![Sign-in activity: last signed in, where you are signed in, and sign-in history](img/signin-activity-member.png)

* **Last signed in** -- your previous sign-in (not the current one): when, how and where.
* **Where you are signed in** -- every browser and phone that is still signed in, with when it signed in and when it was last used. Your current browser shows **This session**.
* **Sign-in history (last 90 days)** -- every sign-in, newest first, 20 per page.

Each row shows:

| Column | What it means |
|---|---|
| Sign-in | How you signed in: `Password`, `Google`, `Apple`, `Library SSO`, `From Librarika.com` (you opened the library from *My Libraries*), `Email link`. **(app)** means the mobile app. |
| Where | The library, or `Librarika.com`. For the app, the libraries you opened in the app. |
| Device | The browser and system (for example *Chrome on Windows*), or the phone's name for the app. |
| IP address | Your internet address with the last part hidden (for example `203.0.113.x`). |
| Status | `Signed in`, `Signed out`, `Signed out from another device`, `Password changed`, `Expired`, or `Signed out for safety`. |

Times are shown in the timezone of your Account Settings.

### Sign out a device

* Click `Sign out` next to a session in **Where you are signed in**. That browser or phone is signed out right away.
* Click `Sign out everywhere else` to sign out every session except the one you are using.
* A phone you sign out also stops receiving that account's notifications.

To sign out other sessions you must be signed in with your password, Google or Apple, not with SSO.

### Don't recognise a sign-in?

1. Click **Change your password** (just above the history) and choose a new password.
2. Changing your password **signs out every other session** automatically, including the mobile app.
3. Check the **SSO sign-in** list and untick any library you don't use.

### "Librarika support accessed your account"

When you ask Librarika support for help, a support person may sign in to your account to look at a problem. That visit appears in your history as **Librarika support accessed your account**, without a device or address. It never counts as your own use of a library.

---

## What your library's administrators can see

A library's administrators see only one thing about your sign-ins: a **Last active** column on their **Users** and **Members** lists. It shows the last time you signed in to **their** library or opened it in the app.

![Users list with the Last active column](img/users-last-active-column.png)

They can't see your history, your devices, your addresses or your activity in other libraries. Sign-ins by Librarika support are never counted.

---

## The mobile app

The Librarika app signs you in to your account, then you pick a library.

* The app offers the same choices as the website: password, **Google**, **Apple** and your library's **SSO**.
* You stay signed in. The app renews its access in the background, so you don't need to sign in again every day.
* `Sign out` in the app signs that phone out on Librarika too, and it stops getting your notifications.
* Each phone appears in **Where you are signed in** with its name (for example *iPhone 15 · iOS 18*), so you can sign out a lost phone from the website.

---

## Your privacy

* Sign-in records are kept for **90 days**, then deleted automatically.
* The full internet address is kept for 30 days to investigate misuse, then shortened. You always see it shortened.
* Deleting your account deletes your sign-in history.
* See the [Privacy Policy](https://librarika.com/spages/privacy-policy) for details.

---

## FAQ

**Why does Google say no account is associated with my Google account?**

Google signs you in only to a Librarika account with the same email address. Sign in with your password, or ask your library which email your account uses.

**I used Apple's "Hide My Email". Why can't I sign in with Apple?**

Apple then gives Librarika a private relay address that doesn't match your Librarika email. Sign in with your password, or choose **Share My Email** the next time Apple asks.

**Can I use my school or work password in Librarika?**

Only through the library's **SSO** button, if your library uses SSO. The Librarika password is a separate password that you create yourself.

**Why can't I sign in with my password to my library any more?**

Your library may allow **SSO only** on its website. Use the SSO (key) button. Your password still works on librarika.com and in other libraries.

**I signed out on my phone, but it still shows as signed in. Why?**

Older versions of the app only signed out on the phone itself. Click `Sign out` next to that phone in **Where you are signed in** to end it on Librarika too.

**What does "Signed out for safety" mean?**

The app's sign-in was used in a way that looked like a copy on another device, so Librarika signed that session out to protect your account. Sign in again on your phone.

**Why is part of my IP address hidden?**

For your privacy. A shortened address is enough to see roughly where a sign-in came from.

**Can I delete my sign-in history?**

It is deleted automatically after 90 days, and all of it is deleted with your account.

**Can my library's administrators see my sign-ins?**

They see only when you were last active in their library. They can't see your history, devices or addresses.

**Why is "Sign out everywhere else" missing?**

You are signed in only once, or you signed in with SSO. Sign in with your password, Google or Apple to sign out other sessions.
