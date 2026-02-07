# SIP2 Integration

For libraries that need physical self-checkout stations -- such as school libraries, public libraries, or corporate libraries with walk-in access -- Librarika supports the **SIP2 protocol** for connecting self-checkout kiosks and other automation devices.

If you are looking for browser-based self-checkout without any hardware, see [Online Self-Service](self-service.md#online-self-service) instead.

## What is SIP2?

SIP2 (Standard Interchange Protocol 2) is an industry-standard protocol used by libraries worldwide to communicate between self-service devices (such as self-checkout kiosks, RFID gates, and automated book sorters) and the library management system. SIP2 allows these devices to perform checkouts, check-ins, and patron lookups without requiring direct access to the library dashboard.

## Requirements

To use SIP2-based self-checkout, you will need:

* A **paid Librarika plan** (Basic Pro, Silver, or Gold).
* A **SIP2 license** -- SIP2 is licensed separately on a per-terminal basis. The Gold plan includes 1 SIP2 terminal by default; for other plans, you need to purchase a SIP2 license. Contact Librarika support for pricing.
* **Kiosk hardware** -- A computer or tablet to serve as the self-checkout terminal.
* A **barcode scanner** -- To scan member IDs and item barcodes.
* **SIP2-compatible kiosk software** -- Software that connects to Librarika via the SIP2 protocol (see [Librarika Kiosk App](#librarika-kiosk-app-coming-soon) below).

## Plan & Licensing

SIP2 is licensed separately on a per-terminal basis. Each terminal that connects to Librarika requires its own SIP2 license.

* **Gold Plan** -- Includes 1 SIP2 terminal by default.
* **Basic Pro / Silver Plans** -- SIP2 licenses must be purchased separately.
* **Additional terminals** -- Available for all paid plans with per-terminal pricing. Contact Librarika support for pricing details.

## Connection Details

* **Protocol**: SIP2 over TLS (encrypted)
* **Port**: 6009
* **Activation**: SIP2 connections must be manually activated by Librarika staff. Please contact support after subscribing to get your SIP2 terminal set up.

## Setup Steps

1. **Subscribe** to a paid Librarika plan (Basic Pro, Silver, or Gold).
2. **Contact Librarika support** to purchase a SIP2 license (if not included in your plan) and request activation. Provide the number of terminals you need.
3. **Configure your kiosk software** with the SIP2 connection details provided by Librarika staff.
4. **Print barcode labels** for your catalog items and member cards. See [Barcode Labels](barcode-labels.md) for instructions.
5. **Test** the connection by performing a test checkout and check-in at your kiosk.

## Librarika Kiosk App (Coming Soon)

Librarika is developing its own kiosk application for self-checkout terminals. The app is designed to work seamlessly with Librarika's SIP2 service and will include:

* **Patron login with barcode scanner** -- Members scan their library card to log in.
* **Multi-item checkout and return** -- Check out or return multiple items in a single session.
* **Session auto-logout** -- Automatically logs out the patron after a period of inactivity.
* **Admin panel** -- Configure branding, timeouts, receipt printing, and other settings.
* **Cross-platform** -- Built with Electron and React, available for Windows, Mac, and Linux.

Stay tuned for updates on the Librarika Kiosk App release.

## FAQ

**Is SIP2 available on the free plan?**

No. SIP2 requires a paid plan (Basic Pro, Silver, or Gold) and a separate SIP2 license purchased on a per-terminal basis. The Gold plan includes 1 SIP2 terminal by default; other plans require purchasing the license separately.

**Do I need a barcode scanner?**

Yes. SIP2 kiosk-based checkout requires a barcode scanner to scan member IDs and item barcodes. If you don't need hardware-based checkout, consider using [Online Self-Service](self-checkout.md#online-self-service) instead -- it works from any browser with no scanner needed.

**Can I use third-party kiosk software?**

Yes. Any SIP2-compatible kiosk software can connect to Librarika. Librarika is also developing its own [Kiosk App](#librarika-kiosk-app-coming-soon) for a seamless experience.
