# Sign-in & Security

This page explains the different ways to sign in to Librarika, how to choose a good password, how to turn on two-step verification, how to see where your account is signed in, and how to sign out of a device you don't recognise. It is written for everyone: library staff, members and people who only use the mobile app.

* **Members:** start with the [quick guide for members](#quick-guide-for-members).
* **Library administrators:** see [For library administrators](#for-library-administrators).

Your **Librarika account** belongs to you, not to one library. You use the same account on [librarika.com](https://librarika.com), in every library you belong to and in the mobile app.

---

## Quick guide for members

* **Sign in:** on your library's login page, enter your email and your Librarika password, or use Google, Apple or your library's SSO button. See [Ways to sign in](#ways-to-sign-in).
* **Forgot your password:** click `Forgot password?` on the login page and follow the link in the email. The link works once, for one hour. See [Forgot your password?](#forgot-your-password).
* **Choose a good password:** at least 15 characters. A few unrelated words are easy to remember and hard to guess. See [Your password](#your-password).
* **Turn on two-step verification:** `My Account` > `Account Settings` > **Two-step verification** > `Turn on`. You need an authenticator app on your phone. Save your recovery codes. See [Two-step verification](#two-step-verification).
* **Lost your phone:** sign in with one of your recovery codes. No recovery codes? Contact your library or Librarika support. See [Lost your phone?](#lost-your-phone).

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

The same page has your [password](#change-your-password) and [two-step verification](#two-step-verification) settings.

If you signed in **with SSO**, you can look at these settings but not change them. You will see *"You signed in with SSO. Sign in with your password or Google to …"*. This protects your account: whoever controls an SSO login can't change how your account signs in.

---

## Your password

Librarika's password rules are part of security improvements based on industry standards. Long passwords protect you better than short, complicated ones, so the rules ask for length and leave the rest to you.

### What makes a good password

When you choose a new password (when you join, change it or reset it), it must:

* have **at least 15 characters**, or **at least 12** if you have [two-step verification](#two-step-verification) turned on. Your library may ask for more (see [Password length](#password-length));
* not be a **common password** or one that has appeared in a **data breach** somewhere on the internet;
* not contain your **username, email address or name**;
* not contain your **library's name** or the word "Librarika";
* not be one character or a short pattern repeated (such as `aaaa` or `abab`), or a simple sequence (such as `abcdef` or `123456`);
* not be the same as your **current password** or one of your **last 5 passwords**.

**Tip:** a few unrelated words make a strong password that is easy to remember, for example *maple river lantern cobalt* (don't use this one). **Spaces and any characters are allowed**, including letters from any language. You don't need to add symbols or capital letters.

### The strength meter

Under the **New password** field you see the rules, and as you type, a strength bar.

![Strength meter for a short, common password](img/signin-password-meter-weak.png)

* **Strength** goes from *Very weak* to *Very strong*. It is advice: a stronger password is harder to guess.
* Below it you may see tips, such as *"Add more words that are less common."*
* Rules your password doesn't meet yet are listed in red with a cross. When every rule is met, you see **Meets every rule.** in green.
* Click **Show password** to see what you typed.

![A long password made of four words: Very strong, Meets every rule](img/signin-password-meter-strong.png)

The check runs in your browser, so nothing you type is sent anywhere until you save. When you save, Librarika checks the rules again. If the password is refused, you see why, for example *"You used this password recently. Please choose a different one."*

### Your current password keeps working

The new rules apply only when you **choose a new password**. The password you have today keeps working until you change it, unless Librarika or your library asks you to [choose a new one](#choose-a-new-password).

### Change your password

1. Open your settings: members click `My Account` > `Account Settings`; staff click the settings menu (gear icon) > `Settings` and open the `Change Password` tab.
2. Enter your **Current password**, then the **New password** twice.
3. Click `Save Settings`.

If you have two-step verification on, Librarika may first ask you to [confirm it's you](#confirm-its-you).

When your password changes:

* every **other** browser and phone is **signed out**, including the mobile app. The browser you are using stays signed in;
* devices where you ticked *"Don't ask again on this device for 30 days"* ask for your two-step code again;
* you get an **email** telling you that your password was changed. If you didn't change it, use the link in that email to reset your password straight away.

### Forgot your password?

1. On the login page, click `Forgot password?`.
2. Enter the email address you use to sign in and click `Email me a link`.
3. You see *"If an account exists for that email address, we have sent a link to reset your password."* You see the same message whether or not the address has an account, so nobody can use this page to find out who has one.
4. Open the email and click the link. The link works **once** and **expires after one hour**. If it has expired, ask for a new one.
5. Choose your new password, enter it again and click `Save new password`.

Resetting your password signs you out on your other devices. It doesn't turn off two-step verification: when you next sign in, you still enter a code from your app (or a [recovery code](#recovery-codes)).

If you don't receive the email, check your spam folder. If you still have no email, ask your library which email address your account uses.

### Choose a new password

Sometimes Librarika shows **Choose a new password** right after you sign in, with *"Your account needs a new password before you go on."* This happens when:

* Librarika support asked you to change it, for example after resetting your two-step verification;
* your library asked everyone to choose a new password (see [Ask for a new password](#ask-for-a-new-password));
* Librarika found that your password appeared in a data breach.

Enter a new password twice and click `Save password`. If you'd rather do it later, click `Sign out`; you will be asked again at your next sign-in.

In the mobile app you may see *"You need to change your password. Please sign in on the Librarika website to change it, then sign in to the app again."* Do that on the website first, then sign in to the app.

### Too many wrong passwords

To protect your account from people guessing passwords, Librarika slows down repeated failed sign-ins:

* After a couple of wrong passwords, the login page asks you to complete a **captcha** ("I'm not a robot" check).
* After more wrong passwords, you have to wait a little before trying again. You see *"Please wait 30 seconds; retrying sooner extends the wait."* (the number of seconds varies). Wait for that time, then try again. Trying sooner makes the wait longer.
* If someone keeps trying wrong passwords on your account, you get an **email** about it. If that wasn't you, nobody has got in: the email has a link to reset your password if you want to be safe.

If you are not sure of your password, use [Forgot password?](#forgot-your-password) instead of guessing.

---

## Two-step verification

Two-step verification adds a second step to signing in with your password. After your password, you enter a **6-digit code** from an **authenticator app** on your phone. The code changes every 30 seconds.

It keeps your account safe **even if someone learns your password**: without your phone they can't sign in.

### What you need

An authenticator app on your phone, for example **Google Authenticator**, **Microsoft Authenticator** or **1Password**. Most authenticator apps work. The app works without an internet connection and doesn't need your phone number.

### Turn on two-step verification

1. Open your settings: members click `My Account` > `Account Settings`; staff click the settings menu (gear icon) > `Settings`.
2. Find **Two-step verification** and click `Turn on`.

	![Two-step verification section in Settings, showing Off and a Turn on button](img/signin-2sv-settings-off.png)

3. Click `Turn on two-step verification`.

	![Two-step verification page when it is off](img/signin-2sv-page-off.png)

4. Librarika may ask you to [confirm it's you](#confirm-its-you) first.
5. Follow the three steps on the page:
	* **Get an authenticator app** on your phone.
	* **Scan this QR code**: in the app, add an account and point your camera at the code. Can't scan it? Type the key shown under the code into the app instead.
	* **Enter the code from the app** in the **6-digit code** field and click `Turn on`.

	![Turn on two-step verification: get an app, scan the QR code, enter the code](img/signin-2sv-turn-on.png)

	If you see *"That code is not right. Please check the time on your phone and try again."*, wait for the next code. Make sure your phone's date and time are set automatically.

6. Save your **10 recovery codes** (see below), then click `I have saved them`.

When two-step verification is turned on (or off), you get an email, and your other browsers and phones are signed out.

### Recovery codes

Recovery codes let you sign in if you lose your phone. You get **10 codes**, and **each one works once**.

![Recovery codes, shown once, with Copy, Download and Print buttons](img/signin-2sv-recovery-codes.png)

* The codes are shown **only once**. Click `Copy`, `Download` or `Print` and keep them somewhere safe, such as a password manager or a printed sheet at home. Don't keep them only on the phone that has your authenticator app.
* To use one, type it into the code field when you sign in, instead of the 6-digit code.
* When you use a recovery code, you get an email about it.
* The two-step verification page shows how many codes you have left.

To get new codes, open the **Two-step verification** page, click `New recovery codes`, then `Make new recovery codes`. New codes replace all your old codes; the old ones stop working.

![Make new recovery codes](img/signin-2sv-new-recovery-codes.png)

### Signing in with two-step verification

1. Sign in with your username (email) and password as usual.
2. On **Enter your code**, open your authenticator app and type the 6-digit code it shows for Librarika into **Code**.
3. If this is your own computer or phone, tick **Don't ask again on this device for 30 days**. Don't tick it on a shared or public computer.
4. Click `Verify`.

**Lost your phone?** Type one of your recovery codes into the same **Code** field.

Good to know:

* If you enter too many wrong codes, you see *"Too many wrong codes. Please sign in again."* After many wrong codes you have to wait: *"Too many wrong codes. Please try again in an hour."*
* Signing in with **Google**, **Apple** or your library's **SSO** usually doesn't ask for the code, because those services have their own checks. Your library (or Librarika) can choose to ask for the code after those sign-ins too.
* Changing your password, or turning two-step verification off, makes every device ask for the code again.

### Manage two-step verification

When two-step verification is on, the section in your settings shows **On** and how many recovery codes you have left. Click `Manage`.

![Two-step verification page when it is on](img/signin-2sv-page-on.png)

* **Set up a new phone** -- move your codes to a new phone. Scan the new QR code with the new phone and enter its code, then click `Use this phone`. Your current phone keeps working until you confirm the new one; after that, the old phone's codes stop working.
* **New recovery codes** -- replace your recovery codes (see above).
* **Turn off two-step verification** -- see below.

### Turn off two-step verification

1. On the **Two-step verification** page, click `Turn off two-step verification`.
2. [Confirm it's you](#confirm-its-you) with your password and a code.
3. Click `Turn off`.

![Turn off two-step verification](img/signin-2sv-turn-off.png)

After that, signing in needs only your password, and your authenticator app and recovery codes stop working. Your **next** password must have at least **15 characters**; the password you have now keeps working.

If your library requires two-step verification, the page says *"Two-step verification is required for your account and cannot be turned off."*

### When your library requires it

A library can require two-step verification for its staff, or for staff and members. If you need it and haven't set it up yet, Librarika asks you after you sign in with your password: **Set up two-step verification** -- *"Your account needs it to finish signing in."* Follow the same three steps as above, save your recovery codes and click `I have saved them, continue`.

If you belong to several libraries and **any** of them requires it, you need it for your whole account.

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

## Lost your phone?

* **You still have your recovery codes:** sign in with a recovery code instead of the 6-digit code. Then open **Two-step verification** and click `Set up a new phone`.
* **You still have your old phone** but are getting a new one: use `Set up a new phone` before you reset or give away the old phone.
* **You have neither your phone nor your recovery codes:** contact your library or [Librarika support](https://librarika.com/spages/contact). Librarika support can turn off two-step verification for your account **after checking who you are**. When they do, you are signed out everywhere, you get an email, and at your next sign-in you [choose a new password](#choose-a-new-password). Then turn two-step verification on again.

Your library's staff can't turn off two-step verification for you, but they can help you contact Librarika support.

If your phone was lost or stolen, also [sign it out](#sign-out-a-device) in **Where you are signed in**.

---

## Emails about your account

Librarika emails you when something important happens to your account, so you notice if it wasn't you:

* your password was changed;
* someone signed in to your account from a **new device or browser**;
* there were many **failed sign-in attempts** on your account;
* two-step verification was turned on or off;
* a **recovery code** was used.

If you get one of these emails and it wasn't you, [reset your password](#forgot-your-password) right away and check your [Sign-in activity](#sign-in-activity).

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
4. Turn on [two-step verification](#two-step-verification), so a password alone is no longer enough to sign in.

### "Librarika support accessed your account"

When you ask Librarika support for help, a support person may sign in to your account to look at a problem. That visit appears in your history as **Librarika support accessed your account**, without a device or address. It never counts as your own use of a library.

---

## What your library's administrators can see

A library's administrators see only one thing about your sign-ins: a **Last active** column on their **Users** and **Members** lists. It shows the last time you signed in to **their** library or opened it in the app.

![Users list with the Last active column](img/users-last-active-column.png)

They can't see your history, your devices, your addresses or your activity in other libraries. They also can't see your password, whether you use two-step verification, or your recovery codes. Sign-ins by Librarika support are never counted.

---

## For library administrators

### Sign-in security

Library administrators can set how staff and members of their library sign in. Go to **Preferences** and click `Sign-in security`.

![Sign-in security button on the Preferences page](img/libraries-preferences-sign-in-security-button.png)

**Availability:** you can change these settings on the **Gold**, **Platinum** and **Unlimited** plans. On other plans the settings are shown but can't be changed, and Librarika's own settings apply.

![The library's Sign-in security page](img/libraries-sign-in-security.png)

#### Two-step verification

* **Who needs it** -- choose one:
	* `Optional: each person chooses` -- the default. Everyone can turn on [two-step verification](#two-step-verification) for themselves.
	* `Required for staff` -- everyone with a role in your library (librarians, administrators and other staff) must use it.
	* `Required for staff and members` -- everyone, including members who can sign in.
* **Also ask for the two-step code after signing in with Google, Apple or the library's SSO** -- by default, people who sign in with Google, Apple or SSO aren't asked for the code, because those services usually have their own two-step check. Tick this to ask for the code anyway. It only applies to people who have turned two-step verification on. This option is shown only when it is available for your library.

When a requirement is on, a person who needs it and hasn't set it up is asked to set it up the next time they sign in with their password. They can't turn it off while it is required.

The requirement follows the person: if someone belongs to several libraries and any one of them requires two-step verification, they need it for their whole account.

#### Password length

* **Minimum without two-step verification** and **Minimum with two-step verification** -- leave them empty to use Librarika's minimums (15 and 12 characters). You can only **raise** them.
* The minimums apply to new passwords of your library's staff and members, and to new accounts that join your library. Existing passwords keep working until they are changed.
* Someone who belongs to several libraries gets the **highest** minimum of all their libraries.

#### Ask for a new password

* **Ask for a new password if it was set before** -- enter a date as `YYYY-MM-DD`. Staff and members whose password was set before that date [choose a new one](#choose-a-new-password) the next time they sign in with their password. Leave it empty for none.
* Use it, for example, if you think passwords may have leaked. If your library is on a plan where you can't change this setting and you need everyone to choose new passwords, ask [Librarika support](https://librarika.com/spages/contact) to set the date for you.

Click `Save` when you are done.

#### "Not enforced yet"

A setting may show **Not enforced yet: for now, sign-ins are only recorded where it would apply.** This means Librarika is still rolling out the feature. You can save the setting now. Until it is enforced, nobody is stopped from signing in; Librarika only records the sign-ins where it would apply. Once it is enforced, the note disappears and the setting takes effect.

### Good practice for your library

* **Require two-step verification for staff.** Staff accounts can change your catalog, members and settings, so they need the most protection.
* **Before requiring it for everyone, tell your members.** Explain that they will need an authenticator app on their phone and should save their recovery codes. Point them to the [quick guide for members](#quick-guide-for-members).
* **Members who use the mobile app:** if the app asks them to update after they turn on two-step verification, they can use your library's website until they do (see [The mobile app](#the-mobile-app)).

### Helping someone who can't sign in

* **Forgot their password:** ask them to click `Forgot password?` on the login page. Staff can't see or set anyone's password.
* **Lost their phone, but has recovery codes:** they sign in with a recovery code, then set up their new phone.
* **Lost their phone and their recovery codes:** they contact [Librarika support](https://librarika.com/spages/contact). Support turns off two-step verification after checking who they are; they then choose a new password at their next sign-in. Library staff can't turn off someone's two-step verification.
* **Waiting after too many wrong passwords:** the wait is short. Ask them to wait, then try once, or use `Forgot password?`.

Library administrators don't see whether someone has two-step verification on, and can't see their password, recovery codes, sign-in history or devices. They see only the **Last active** column (see [What your library's administrators can see](#what-your-librarys-administrators-can-see)).

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

**Why is my old password not accepted when I change it?**

Your new password must be different from your current password and from your last 5 passwords. You see *"You used this password recently. Please choose a different one."* Choose a new one; a few unrelated words work well.

**Why is my new password refused?**

The message says which rule it doesn't meet: too short (at least 15 characters, or 12 with two-step verification), a common or breached password, or it contains your name, email, the library's name or "Librarika". See [What makes a good password](#what-makes-a-good-password).

**Do I have to change my password now that the rules are stricter?**

No. Your current password keeps working. The new rules apply the next time you choose a password, unless Librarika or your library asks you to [choose a new one](#choose-a-new-password).

**Why does Librarika ask me to choose a new password?**

Librarika support or your library asked for it, for example after resetting your two-step verification or after a possible leak, or your password was found in a data breach. Choose a new one to continue. See [Choose a new password](#choose-a-new-password).

**My reset link doesn't work. Why?**

A reset link works once and expires after one hour. Ask for a new one with `Forgot password?`.

**Why do I have to wait before signing in?**

Too many wrong passwords were entered for your account. Librarika slows down further attempts to stop people from guessing passwords. Wait for the time shown, then try again, or use `Forgot password?`. See [Too many wrong passwords](#too-many-wrong-passwords).

**Do I need two-step verification?**

It is optional unless your library requires it. We recommend it for everyone, and especially for library staff: it protects your account even if someone learns your password.

**Which authenticator app should I use?**

Any common authenticator app works, for example Google Authenticator, Microsoft Authenticator or 1Password.

**Where are my recovery codes?**

Librarika shows them only once, when you turn on two-step verification or make new ones. If you didn't save them, open **Two-step verification** and click `New recovery codes` to make a new set; the old ones stop working.

**I lost my phone. What do I do?**

Sign in with one of your recovery codes, then use `Set up a new phone`. If you have no recovery codes either, contact your library or Librarika support; support can turn off two-step verification after checking who you are. See [Lost your phone?](#lost-your-phone).

**I got a new phone. How do I move my codes?**

Before you reset the old phone, open **Two-step verification**, click `Set up a new phone` and scan the new QR code with the new phone. The old phone keeps working until you confirm the new one.

**My code is always "not right". Why?**

The codes depend on your phone's clock. Set your phone's date and time to update automatically, then try the newest code.

**Why can't I turn off two-step verification?**

Your library (or one of your libraries) requires it. The page says *"Two-step verification is required for your account and cannot be turned off."*

**Why does Librarika ask me to confirm it's me?**

You are about to change something important, such as your password, email, two-step verification or account. Enter your password and code, or ask for an emailed link if you sign in with SSO, Google or Apple. See [Confirm it's you](#confirm-its-you).

**Does signing in with Google, Apple or SSO ask for my code?**

Usually not, because those services have their own checks. Your library can choose to ask for the code after those sign-ins too.

**The app says "Please update the Librarika app to sign in". What do I do?**

Your account uses two-step verification and your version of the app can't ask for the code. Update the app, or use the library's website until an update is available.

**Can my library see my password or recovery codes?**

No. Nobody at your library can see your password, your recovery codes or whether you use two-step verification.
