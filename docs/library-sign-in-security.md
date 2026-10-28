# Library sign-in security

**Who this is for:** library administrators.

**What you can do here:** decide how staff and members of your library sign in: require two-step verification, set minimum password lengths, and ask everyone for a new password.

## Open the Sign-in security page

Library administrators can set how staff and members of their library sign in. Go to **Preferences** and click `Sign-in security`.

![Sign-in security button on the Preferences page](img/libraries-preferences-sign-in-security-button.png)

**Availability:** you can change these settings on the **Gold**, **Platinum** and **Unlimited** plans. On other plans the settings are shown but can't be changed, and Librarika's own settings apply.

![The library's Sign-in security page](img/libraries-sign-in-security.png)

## Two-step verification

* **Who needs it** -- choose one:
	* `Optional: each person chooses` -- the default. Everyone can turn on [two-step verification](#two-step-verification) for themselves.
	* `Required for staff` -- everyone with a role in your library (librarians, administrators and other staff) must use it.
	* `Required for staff and members` -- everyone, including members who can sign in.
* **Also ask for the two-step code after signing in with Google, Apple or the library's SSO** -- by default, people who sign in with Google, Apple or SSO aren't asked for the code, because those services usually have their own two-step check. Tick this to ask for the code anyway. It only applies to people who have turned two-step verification on. This option is shown only when it is available for your library.

When a requirement is on, a person who needs it and hasn't set it up is asked to set it up the next time they sign in with their password. They can't turn it off while it is required.

The requirement follows the person: if someone belongs to several libraries and any one of them requires two-step verification, they need it for their whole account.

## Password length

* **Minimum without two-step verification** and **Minimum with two-step verification** -- leave them empty to use Librarika's minimums (15 and 12 characters). You can only **raise** them.
* The minimums apply to new passwords of your library's staff and members, and to new accounts that join your library. Existing passwords keep working until they are changed.
* Someone who belongs to several libraries gets the **highest** minimum of all their libraries.

## Ask for a new password

* **Ask for a new password if it was set before** -- enter a date as `YYYY-MM-DD`. Staff and members whose password was set before that date [choose a new one](passwords.md#choose-a-new-password) the next time they sign in with their password. Leave it empty for none.
* Use it, for example, if you think passwords may have leaked. If your library is on a plan where you can't change this setting and you need everyone to choose new passwords, ask [Librarika support](https://librarika.com/spages/contact) to set the date for you.

Click `Save` when you are done.

## "Not enforced yet"

A setting may show **Not enforced yet: for now, sign-ins are only recorded where it would apply.** This means Librarika is still rolling out the feature. You can save the setting now. Until it is enforced, nobody is stopped from signing in; Librarika only records the sign-ins where it would apply. Once it is enforced, the note disappears and the setting takes effect.

## Good practice for your library

* **Require two-step verification for staff.** Staff accounts can change your catalog, members and settings, so they need the most protection.
* **Before requiring it for everyone, tell your members.** Explain that they will need an authenticator app on their phone and should save their recovery codes. Point them to the [quick guide for members](sign-in-and-security.md#quick-guide-for-members).
* **Members who use the mobile app:** if the app asks them to update after they turn on two-step verification, they can use your library's website until they do (see [The mobile app](signing-in.md#the-mobile-app)).
