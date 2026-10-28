# SIP2 Integration

For libraries that need physical self-checkout stations -- such as school libraries, public libraries, or corporate libraries with walk-in access -- Librarika supports the **SIP2 protocol** for connecting self-checkout kiosks and other automation devices.

If you are looking for browser-based self-checkout without any hardware, see [Online Self-Service](self-service.md#online-self-service) instead.

## What is SIP2?

SIP2 (Standard Interchange Protocol 2) is an industry-standard protocol used by libraries worldwide to communicate between self-service devices (such as self-checkout kiosks, RFID gates, and automated book sorters) and the library management system. SIP2 allows these devices to perform checkouts, check-ins, and patron lookups without requiring direct access to the library dashboard.

## Requirements

To use SIP2-based self-checkout, you will need:

* A **SIP2 licence for each terminal** -- Librarika sets up and licenses each terminal for you. Contact Librarika support for availability on your plan and for pricing.
* A **dedicated staff account for each terminal** -- an active user account in your library that is used only by that terminal, not a person's own login.
* **Kiosk hardware** -- A computer or tablet to serve as the self-checkout terminal.
* A **barcode scanner** -- To scan member IDs and item barcodes.
* **SIP2-compatible kiosk software** -- Software that connects to Librarika via the SIP2 protocol such as the [Librarika Kiosk App](#librarika-kiosk-app) below.

## Licensing

SIP2 is licensed per terminal. Each terminal that connects to Librarika needs its own licence, which Librarika links to the terminal's staff account. A licence runs for a set period (usually a year); after its end date the terminal keeps working only for a short grace period. A licence can also list the IP addresses the terminal may connect from. Contact Librarika support for pricing and to add, move or renew a terminal.

## Connection Details

* **Protocol**: SIP2 over TLS (encrypted)
* **Port**: 6009
* **Institution ID (AO)**: your library's subdomain, for example `mylibrary` for `mylibrary.librarika.com`.
* **Login**: the terminal's dedicated staff account (username and password). Use the account that Librarika support licensed for the terminal: a licensed terminal account is not asked for two-step verification or a new password, but an ordinary staff account is, and a kiosk can't answer. See [Kiosk app](kiosk-app.md#get-a-terminal-licence-and-account).
* **Allowed IPs**: if the licence lists IP addresses, the terminal must connect from one of them.
* **Activation**: SIP2 terminals are set up by Librarika staff. Please contact support to get your SIP2 terminal set up.

## Setup Steps

1. **Create a staff account** in your library for each terminal (see [Users](users.md)).
2. **Contact Librarika support** to license and activate your terminals. Tell them the number of terminals, each terminal's account, and the IP addresses the terminals connect from.
3. **Configure your kiosk software** with the SIP2 connection details provided by Librarika staff.
4. **Print barcode labels** for your catalog items and member cards. See [Barcode Labels](barcode-labels.md) for instructions.
5. **Test** the connection by performing a test checkout and check-in at your kiosk.

## Librarika Kiosk App

Librarika has its own kiosk app for self-checkout terminals. Members scan their library card, then borrow and return items; staff set it up with an admin PIN and can add branding, library hours, auto sign-out and receipt printing.

* For staff: [Kiosk app: setup and management](kiosk-app.md).
* For members: [Using a kiosk](using-a-kiosk.md).
* Downloads and supported systems: the [Librarika Kiosk App](https://librarika.com/spages/librarika-kiosk-app) page.

## FAQ

**Is SIP2 available on the free plan?**

Each SIP2 terminal needs its own licence from Librarika. Contact Librarika support to ask about SIP2 for your plan and about pricing.

**Do I need a barcode scanner?**

Yes. SIP2 kiosk-based checkout requires a barcode scanner to scan member IDs and item barcodes. If you don't need hardware-based checkout, consider using [Online Self-Service](self-service.md) instead -- it works from any browser with no scanner needed.

**Can I use third-party kiosk software?**

Yes. Any SIP2-compatible kiosk software can connect to Librarika. Librarika also has its own [Kiosk app](kiosk-app.md).

**Can two kiosks share one SIP2 licence?**

No. Each terminal has its own licence and signs in with its own active staff account in your library. Use a separate account for each terminal, not a person's own login, because a terminal account is meant for SIP2 use only.

**Where can I see my SIP2 terminals and when their licences end?**

Go to `Manage -> Preferences` and open the `SIP2` tab (it appears once a terminal is licensed for your library). It shows each terminal's allowed IPs, licence end date, status and when it was last used. To add, move or renew a terminal, contact Librarika support.

**Why has my kiosk stopped working?**

Check the status on the `SIP2` tab in Preferences. The licence may have expired (after the end date the terminal keeps working only for a grace period), it may be suspended, or the kiosk may be connecting from an IP address that is not in its allowed list, for example after an internet provider change. Contact Librarika support to renew the licence or update the allowed IPs.

**What can members do at a SIP2 kiosk?**

Members can identify themselves, check out items and return them. Renewals, holds and fee payments are not available through SIP2.

**Do kiosk checkouts follow my circulation rules?**

Yes. The same checks apply as at the desk: an inactive member, a member who has reached their booking quota or dues limit, an item with circulation disabled, an item already issued, or an item on the hold shelf for another member is refused.
