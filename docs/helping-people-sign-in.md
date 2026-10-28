# Helping people who can't sign in

**Who this is for:** library staff and administrators.

**What you can do here:** find the right fix when a member or colleague can't sign in. Nobody at your library can see or set someone's password, turn off their two-step verification or see their recovery codes, so most fixes are steps the person takes themselves.

---

## Forgot their password

Ask them to click `Forgot password?` on the login page, enter their email address and click `Email me a link`. The link works once, for one hour. See [Forgot your password?](passwords.md#forgot-your-password).

* **No email arrives:** they check their spam folder. Then check which email address their account uses: open the member (or user) in Librarika and compare. The reset email goes only to the address of their Librarika account.
* **"Invalid username or password, try again.":** they may be using an old email address, or their account may use a different one than you think.

## Has to wait, or sees a captcha

After two wrong passwords the login page asks for a captcha; after more, they have to wait (*"Please wait 30 seconds; retrying sooner extends the wait."*). The wait is short. Ask them to wait for the time shown and try once, or to use `Forgot password?` instead of guessing. See [Too many wrong passwords](passwords.md#too-many-wrong-passwords).

## Asked to choose a new password

If Librarika shows **Choose a new password** after they sign in, they choose one there. Your library may have asked for it (see [Ask for a new password](library-sign-in-security.md#ask-for-a-new-password)). In the mobile app they do it on the website first. See [Choose a new password](passwords.md#choose-a-new-password).

## Their new password is refused

The message says which rule it doesn't meet. Suggest a few unrelated words, at least 15 characters (12 with two-step verification, or more if your library raised the minimum). See [What makes a good password](passwords.md#what-makes-a-good-password).

## Lost their phone (two-step verification)

* **Has recovery codes:** they sign in with a recovery code instead of the 6-digit code, then use `Set up a new phone`.
* **Has neither phone nor recovery codes:** they contact [Librarika support](https://librarika.com/spages/contact). Support turns off two-step verification after checking who they are; they then choose a new password at their next sign-in. Library staff can't do this for them.

See [Lost your phone?](two-step-verification.md#lost-your-phone).

## Asked to set up two-step verification

If your library requires two-step verification, people who haven't set it up are asked to at their next password sign-in. They need an authenticator app on their phone. In the mobile app they set it up on the website first. See [When your library requires it](two-step-verification.md#when-your-library-requires-it).

## Hasn't joined yet

* **Invitation expired** (*"This invitation has expired. Please ask the library to send it again."*): invitations work for 30 days. Re-send it from the Members list (`Re-send Invite`) or the member's page (`Re-send Invitation Email`).
* **"Member login is turned off for this membership. Please contact the library.":** turn on member access for them (see [Members](members.md#enable-member-access)).
* **"Please verify your email address in order to login.":** their account's email isn't confirmed yet. They use the link in the confirmation email, or `Forgot password?`, which also confirms it.

See [Member quick start](member-quick-start.md).

## SSO problems

* **"This library's SSO is not allowed to sign in to your account yet. …":** their account is also used elsewhere. They sign in once with their password or Google and tick your library under **SSO sign-in** in their settings.
* **"This library allows sign-in with its SSO only. Please sign in with SSO.":** your library allows SSO only. They use the `Sign in with SSO` button.
* **"Your SSO login is either invalid or expired.":** they try again from your library's login page. If it keeps happening, check your SSO settings.

See [Single sign-on](sso-saml.md#troubleshooting).

## Mobile app

Most app problems have a message with a button, such as `Change password on the website` or `Update the app`. See [Troubleshooting the app](app-troubleshooting.md).

## Kiosks

A kiosk signs in with its own licensed terminal account, never a person's login. If every member at a kiosk sees *"Your account is blocked. Please see library staff."*, the problem is usually the kiosk, not the members. See [Kiosk troubleshooting](kiosk-app.md#troubleshooting).

---

## What you can and can't see

Library administrators see only the **Last active** column on their **Users** and **Members** lists: *"Their last sign-in to this library, or use of it in the app, by themselves (never Librarika support)"*. You can't see whether someone has two-step verification on, their password, recovery codes, sign-in history or devices. See [What your library's administrators can see](sign-in-activity.md#what-your-librarys-administrators-can-see).
