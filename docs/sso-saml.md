# SSO / SAML Integration

Single Sign-On (SSO) allows your library members to log in using their existing organizational credentials (e.g., school or company login) instead of creating separate Librarika passwords. Librarika supports SSO through the **SAML 2.0** protocol.

## Benefits

* **Simplified login** -- Members use their existing organizational username and password to sign in to your library.
* **Centralized authentication** -- User access is managed through your organization's Identity Provider (IdP). When a user is removed from your organization, they automatically lose access to the library.
* **Enhanced security** -- Authentication is handled by your organization's secure login system, supporting multi-factor authentication and other security policies.

## Plan Availability

SSO/SAML integration is available on **Silver** and **Gold** plans only.

## Supported Identity Providers

Librarika supports any SAML 2.0 compliant Identity Provider, including:

* Microsoft Azure AD (Entra ID)
* Google Workspace
* Okta
* OneLogin
* Auth0
* Ping Identity
* ADFS (Active Directory Federation Services)
* Shibboleth

If your Identity Provider supports SAML 2.0, it should work with Librarika even if it is not listed above.

---

## How SSO Works

1. A member opens your library's login page and clicks the **SSO** button (the key icon, next to Google and Apple).
2. The member is redirected to your organization's Identity Provider (IdP) login page.
3. The member enters their organizational credentials (e.g., school email and password).
4. The Identity Provider authenticates the member and sends a SAML response back to Librarika.
5. Librarika validates the response and logs the member in automatically.

---

## Setup Instructions

Setting up SSO requires configuration on both sides -- your Identity Provider and Librarika. Follow these steps:

### Step 1: Access SSO Settings in Librarika

* Go to **Dashboard > Manage > Preferences**.
* Click on the `SSO` tab.

	![Library preference SSO form](img/library-preference-sso.png)

* You will see the following fields provided by Librarika:
	* **ACS URL** (Assertion Consumer Service URL) -- The endpoint where your IdP sends the SAML response.
	* **ACS Entity ID** -- The identifier for Librarika as the Service Provider.

* Copy these values -- you will need them in the next step.

**Note:** The URLs shown will contain your library's subdomain (e.g., `yourlibrary.librarika.com`).

### Step 2: Configure Your Identity Provider

In your Identity Provider's admin console, create a new SAML application with the following settings:

* **ACS URL / Reply URL** -- Paste the ACS URL from Step 1.
* **Entity ID / Audience URI** -- Paste the ACS Entity ID from Step 1.
* **Name ID Format** -- Email address (recommended).

The exact steps vary by provider. Consult your Identity Provider's documentation for creating a SAML application.

### Step 3: Enter IdP Details in Librarika

After configuring your Identity Provider, you will receive the following details. Enter them in the SSO tab in Librarika:

* **SAML Provider** -- Select your SAML provider from the dropdown list.
* **IdP Entity ID** -- The identifier of your Identity Provider (a URI provided by your IdP).
* **IdP SSO Service URL** -- The login endpoint URL where Librarika sends authentication requests.
* **IdP x509 Certificate** -- The public certificate from your IdP, used to verify SAML responses.

You can find these values in the **metadata** of your SAML provider. Most providers offer a metadata XML file or a metadata URL that contains all three values.

### Step 4: Enable SSO and Request Activation

* Check the **Enable SSO** checkbox.
* Click the `Save Preferences` button.
* **Contact Librarika support** to request SSO activation. Librarika staff will review your configuration and activate SSO for your library.

**Important:** SSO is not active immediately after saving. It requires manual review and activation by Librarika staff.

### Step 5 (optional): Allow SSO only

On the same `SSO` tab you can make SSO the only way into your library:

* **SSO only on the website** -- members and staff can sign in to your library's website with SSO only. Anyone signed in another way (password, Google, or from *My Libraries* on librarika.com) is signed out of your library and asked to use SSO. Their Librarika account keeps working on librarika.com and in other libraries.
* **SSO only on the mobile app** -- in the Librarika app, your library can then only be used after signing in with your library's SSO.

Before you switch these on, make sure every member's email in your Identity Provider matches their Librarika email.

---

## Member Login with SSO

Once SSO is activated, members can log in to your library as follows:

1. Go to your library's login page.
2. Click the **SSO** button (the key icon).
3. Enter organizational credentials on the Identity Provider's login page.
4. After successful authentication, the member is redirected back to the library and logged in.

**Who can sign in with SSO:**

* **A person with no Librarika account yet:** SSO creates their account and sends a member request to your library. They join automatically if `Join member automatically.` is on in your preferences; otherwise the request waits for staff to accept it. If `Enable member access request.` is off, the request is refused.
* **A person who already has a Librarika account** with the same email: SSO signs them in when your library is on their own **SSO sign-in** list (in their settings). Your library is added to the list automatically when SSO created the account, or when the account belongs only to your library. Otherwise they see *"This library's SSO is not allowed to sign in to your account yet. Sign in with your password or Google, then allow this library under Settings…"*. They sign in with their password once, tick your library under **SSO sign-in** in their settings, and SSO works from then on. See [Sign-in & Security](signing-in.md#your-sign-in-settings).

This protects accounts that are used in more than one library: one organisation's SSO can't take over an account it doesn't own.

**Passwords:** people invited to your library still create a **Librarika password** when they accept the invitation. The invitation page explains that it is separate from your organisation's SSO password and why they need it (librarika.com and other libraries don't use your SSO).

---

## SSO in the Mobile App

Members can sign in to the Librarika app with your library's SSO too: on the app's login screen they tap the SSO option and choose your library. If you turned on **SSO only on the mobile app**, this is the only way to use your library in the app.

---

## FAQ

**Can I use SSO with the free plan?**

No. SSO/SAML integration is available on Silver and Gold plans only.

**Is SSO activated immediately after I configure it?**

No. After you save your SSO configuration, you need to contact Librarika support for manual review and activation.

**Can members still log in with their Librarika password after SSO is enabled?**

Yes, unless you switch on **SSO only on the website** (see [Step 5](#step-5-optional-allow-sso-only)). Enabling SSO adds a login method; it doesn't remove the others.

**What if my Identity Provider is not listed in the dropdown?**

If your IdP supports SAML 2.0 but is not in the dropdown list, select the closest option or contact Librarika support for assistance.

**Do members need to be pre-created in Librarika?**

No. A person without a Librarika account gets one at their first SSO sign-in, together with a member request to your library (joined automatically if `Join member automatically.` is on). Existing members sign in with SSO when the email in your Identity Provider matches their Librarika email.

**A member says "This library's SSO is not allowed to sign in to your account yet". What should they do?**

Their account is used outside your library too, so they must allow your library once: sign in with their password or Google, open their settings, tick your library under **SSO sign-in**, and save.

**A member signed in with SSO but can't change their email or settings. Why?**

For safety, a session started with SSO can't change how the account signs in (email, Google, Apple or the SSO list) or sign out other sessions. They sign in with their password or Google to do that.

**Why does an invited member have to create a password if we use SSO?**

The Librarika account is theirs, not the library's: they also use it on librarika.com and in other libraries, where your SSO doesn't sign them in. They can still use SSO for your library.

**Can members use SSO in the mobile app?**

Yes. On the app's login screen they choose SSO and your library. See [SSO in the Mobile App](#sso-in-the-mobile-app).

