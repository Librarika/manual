# Self-Service

Librarika offers two approaches for self-checkout: **Online Self-Service** and **Kiosk-Based Self-Service (SIP2)**. Online self-service allows members to check out and return items directly from their browser or phone, while kiosk-based self-service uses the industry-standard SIP2 protocol to connect physical self-checkout terminals with barcode scanners.

## For members

If your library allows it, you can borrow and return items yourself.

**Borrow an item**

1. Sign in to your library's website and find the item (`Search Catalog`).
2. On the item's page, click `Checkout` next to an available copy. The **Self Checkout** window opens.
3. Check the **From** and **To** dates (you can't go past your library's limit) and click `Submit`.
4. You see *"The item has been checked out successfully. Please return the item on time."*

**Return an item**

1. Click `My Account` and find the item in your current loans.
2. Click `Check-in`. The **Self Check-In** window opens; you can add a comment.
3. Click `Submit`. You see *"The item has been returned successfully…"*

No `Checkout` button? Your library hasn't turned on self-checkout for your membership, or the copy is out. Ask at the desk. Using a kiosk in the library instead? See [Using a kiosk](using-a-kiosk.md).

---

## For library staff

### Overview

| Feature | Online Self-Service | [Kiosk-Based (SIP2)](sip2.md) |
|---|---|---|
| Hardware required | None (browser only) | Kiosk terminal + barcode scanner |
| Barcode scanner needed | No | Yes |
| Plan requirement | All plans (including Free) | A SIP2 licence for each terminal (ask Librarika support about your plan) |
| Setup | Configure in Preferences | Contact Librarika support |
| Best for | Remote access, small libraries | High-traffic libraries, walk-in stations |


### Online self-service

Online self-service allows your library members to check out and return items directly from their browser without any staff involvement. Members simply log in, find the item they want, and click the checkout button.

#### Prerequisites

Before members can use self-service, make sure the following are in place:

* **Member login access enabled** -- Each member must have login access turned on. See [Enable Member Access](members.md#enable-member-access) for instructions.
* **Self-service preferences configured** -- The self-service settings must be enabled in your library preferences (see below).

#### Enable self-service for your library

To enable self-service checkout and check-in for your library members, follow these steps:

* In the sidebar, go to `Manage` > `Preferences`.
* Click on the `Self Service` tab.

	![Library preference self-service form](img/library-preference-self-service.png)

	This picture is from an older version: the tab bar now also has `Hold Queue` (and `SIP2` when your library has terminals). The settings on the tab are the same.

* Configure the following settings:

	* **Enable member checkouts** -- Allow members to check out items by themselves from the catalog.
	* **Enable member check-ins** -- Allow members to return (check-in) items by themselves from their My Account page.
	* **Enable member check-ins for overdue items** -- Allow members to return items even if they are overdue. It works only when **Enable member check-ins** is on. If it is off, overdue items can only be returned by library staff.
	* **Member** -- which members may use self-service: All Members, Regular Members Only or Privileged Members Only.
	* **Checkout Time** -- the default checkout duration in days (default 7).
	* **Checkout Limit** -- the longest checkout a member can choose, in days (default 14).
	* **Checkout Quota** -- the most items a member can have checked out at the same time (default 5). Self-checkout counts every item the member has issued or overdue, including items issued by staff.

* Click the `Save Preferences` button to save your changes.

What members see is described in [For members](#for-members) above.

<a id="how-members-check-out-items"></a><a id="how-members-return-items"></a>

---

### Kiosk-based self-service (SIP2)

For libraries that need physical self-checkout stations with barcode scanners, Librarika supports the industry-standard **SIP2 protocol**. Each SIP2 terminal needs its own licence from Librarika.

For full details on SIP2 requirements, licensing, connection setup, see the [SIP2 integration](sip2.md) page. To set up the Librarika Kiosk App, see [Kiosk app: setup and management](kiosk-app.md); members can read [Using a kiosk](using-a-kiosk.md).

---

## FAQ

**Do I need a barcode scanner for self-checkout?**

Only if you are using [kiosk-based (SIP2)](sip2.md) self-checkout. For online self-service, members check out items through their browser -- no barcode scanner is needed.

**Do I need third-party software for online self-service?**

No. Online self-service is a built-in feature of Librarika. Simply enable it in your library preferences and your members can start using it right away.

**Is SIP2 available on the free plan?**

Each SIP2 terminal needs its own licence from Librarika. Contact Librarika support about SIP2 for your plan and about pricing. See [SIP2 integration](sip2.md).

**Can members check out items from their phone?**

Yes. With online self-service enabled, members can sign in and check out items from any device with a web browser, including smartphones and tablets.

**Why can't a member see the `Checkout` button?**

The `Checkout` button appears next to a copy only when **Enable member checkouts** is on, the member's type matches the **Member** setting, the copy is not already checked out, and the item is marked as circulating. Check these in [Enable Self-Service for Your Library](#enable-self-service-for-your-library).

**Why can't a member return an overdue item themselves?**

If **Enable member check-ins for overdue items** is off, the `Check-in` button is hidden for overdue items in the member's account, and only library staff can check them in. Turn the setting on if you want members to return overdue items themselves.

**Does the Checkout Quota count items checked out by staff?**

Yes. The quota counts every item the member currently has checked out or overdue, no matter who issued it. If a member already has that many items, self-checkout is refused until they return something.

**Can unpaid fees stop a member from checking out?**

Yes, if your library uses [Fees & Payments](fees-payments.md) with **Suspend activity** turned on. When the member's balance reaches the **Suspension Limit**, self-checkout shows "Sorry, you have reached the maximum dues limit."
