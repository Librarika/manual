# Signing in

**Who this is for:** everyone: library staff, members and people who use the mobile app.

**What you can do here:** sign in with a password, Google, Apple or your library's SSO, manage your sign-in settings, and confirm it's you before important changes.

Your **Librarika account** belongs to you, not to one library. You use the same account on [librarika.com](https://librarika.com), in every library you belong to and in the mobile app.

Related pages: [Passwords](passwords.md) · [Two-step verification](two-step-verification.md) · [Sign-in activity & privacy](sign-in-activity.md)

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

* Google and Apple sign you in to the Librarika account with the **same email address**. If you don't have a Librarika account yet, `Sign up with Google` or `Sign up with Apple` on the sign-up page creates one for you, with no new password to remember.
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

The same page has your [password](passwords.md#change-your-password) and [two-step verification](two-step-verification.md) settings.

If you signed in **with SSO**, you can look at these settings but not change them. You will see *"You signed in with SSO. Sign in with your password or Google to …"*. This protects your account: whoever controls an SSO login can't change how your account signs in.

---

## Confirm it's you

Before an important change, Librarika asks you to **confirm it's you**. This stops someone who finds your computer still signed in from taking over your account. You may be asked before you:

* change your password or email address;
* turn two-step verification on or off, set up a new phone, or make new recovery codes;
* remove your account.

![Confirm it's you: password and code, or an emailed link](img/signin-confirm-its-you.png)

* Enter your **Password** and, if two-step verification is on, a **Code** from your app (or a recovery code). Click `Continue`.
* After confirming, you won't be asked again for about **10 minutes**.
* If you signed in with your password just now, you may not be asked at all.

**No password?** If you sign in with SSO, Google or Apple, or don't know your password, click `Email me a confirmation link`. Open the email **in the same browser**; the link works once, for one hour. If two-step verification is on, you then enter a code from your app.

---

## The mobile app

The Librarika app signs you in to your account, then you pick a library.

* The app offers the same choices as the website: password, **Google**, **Apple** and your library's **SSO**.
* You stay signed in. The app renews its access in the background, so you don't need to sign in again every day.
* `Sign out` in the app signs that phone out on Librarika too, and it stops getting your notifications.
* Each phone appears in **Where you are signed in** with its name (for example *iPhone 15 · iOS 18*), so you can sign out a lost phone from the website.

**Two-step verification in the app**

* Turn two-step verification on and off on the website. When you sign in to the app with your password, the app asks for your code (or a recovery code) like the website does.
* If your version of the app can't ask for the code yet, it shows *"Please update the Librarika app to sign in. Your account uses two-step verification."* Update the app from the App Store or Google Play. If no update is available yet, use the library's website in your phone's browser.
* If your account needs two-step verification but you haven't set it up, set it up on the website first, then sign in to the app.
* If Librarika asks you to choose a new password, do it on the website, then sign in to the app again.

---

## FAQ

**Why does Librarika say no account uses my Google or Apple email?**

Google and Apple sign you in only to the Librarika account with the same email address. If your Librarika account uses another email, sign in with your password, or ask your library which email your account uses. If you have no Librarika account yet, use `Sign up with Google` or `Sign up with Apple` on the sign-up page.

**Can I use my school or work password in Librarika?**

Only through the library's **SSO** button, if your library uses SSO. The Librarika password is a separate password that you create yourself.

**Why can't I sign in with my password to my library any more?**

Your library may allow **SSO only** on its website. Use the SSO (key) button. Your password still works on librarika.com and in other libraries.

**Why does Librarika ask me to confirm it's me?**

You are about to change something important, such as your password, email, two-step verification or account. Enter your password and code, or ask for an emailed link if you sign in with SSO, Google or Apple. See [Confirm it's you](#confirm-its-you).
