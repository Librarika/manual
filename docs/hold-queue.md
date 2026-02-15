# Hold Queue

The hold queue feature allows members to place holds on items that are currently checked out or unavailable, and wait in a first-in, first-out (FIFO) queue until the item becomes available. Library staff can manage the hold queue, hold shelf, and fulfill holds through the circulation dashboard. Members can also place and manage their own holds from the catalog and member area.

**Availability:** Hold Queue is available on **Basic Pro**, **Silver**, **Gold**, **Platinum**, and **Unlimited** plans.

---

## Enable Hold Queue

To enable the hold queue feature for your library, please follow the below steps:

* Go to the `Dashboard -> Manage -> Preferences` section.
* Click on the `Hold Queue` tab.
* Check the `Enable hold queue` checkbox to activate the feature.
* Configure the hold queue settings as described below.
* Click on the `Save Preferences` button to save your changes.

### Hold Queue Settings

The following settings are available under the Hold Queue tab in Preferences:

| Setting | Description | Default |
|---------|-------------|---------|
| **Enable hold queue** | Master toggle to enable or disable the hold queue feature for your library. | Off |
| **Member** | Choose which member types can place holds: All Members, Regular Members Only, or Privileged Members Only. | All Members |
| **Hold Quota** | Maximum number of active holds a member can have at a time. | 5 |
| **Allow title-level holds** | Members can place holds on any available copy of a title. When a copy is returned, it will be automatically assigned. | On |
| **Allow copy-level holds** | Members can place holds on a specific copy of a title. | On |
| **Hold Expiration** | Number of days before an unfulfilled hold expires automatically. | 180 |
| **Pickup Window** | Number of days a member has to pick up an item after it becomes ready. | 7 |
| **Fulfillment Mode** | How holds are fulfilled when items are returned. **Auto Assign:** Automatically assign returned items to waiting holds. **Notify & Confirm:** Notify the member and wait for confirmation before assigning. **Staff Manual:** Staff manually assigns items to holds. | Auto Assign |
| **Auto-ready on placement** | When a hold is placed and a copy is currently available, automatically mark the hold as ready for pickup instead of placing it in the queue. | Off |
| **Enable recall** | When a hold is placed, shorten the due date for the current borrower to encourage earlier return. | Off |
| **Recall Period** | Number of days the current borrower has after a recall is triggered. | 7 |
| **Notify when hold is ready** | Send an email notification to the member when their hold is ready for pickup. | On |
| **Notify when hold expires** | Send an email notification to the member when their hold expires. | On |

---

## Hold Queue (Staff)

Library staff can manage all hold-related activities from the Hold Queue section in the Circulations menu.

### View Hold Queue

To view and manage all holds in your library:

* Go to `Dashboard -> Circulations -> Hold Queue`.
* The hold queue list will be displayed with all active holds.
* Use the status dropdown to filter holds by status: **Active**, **Actionable**, **Waiting**, **Ready**, **Suspended**, **Fulfilled**, **Expired**, **Cancelled**, or **All**.
* Use the search box to find holds by title, ISBN, member name, or member number.

**Note:** If the hold queue feature is disabled, a warning message will be displayed with a link to the settings page.

### Place Hold (Staff)

Staff can place holds on behalf of members. To place a hold:

* Go to `Dashboard -> Circulations -> Hold Queue`.
* Click on the `Place Hold` button.
* The Place Hold form will appear.
* Enter the member number or member name. An auto-select list will appear, please select the member from the list.
* Enter the accession number, ISBN, title, or call number of the item. An auto-select list will appear with availability indicators (green = available, red = checked out).
	* If you scan or enter an **accession number**, the system will automatically set the hold as a **copy-level** hold.
	* If you scan or enter an **ISBN** or search by title, the system will set the hold as a **title-level** hold.
* If copy-level holds are enabled, you can optionally select a specific copy from the dropdown.
* Add any notes if needed.
* Click on the `Submit` button to place the hold.

The member will be assigned a queue position and will receive a notification if they have a linked user account.

**Note:** The system will prevent placing a hold if:

* The member has reached their hold quota limit.
* The member already has an active hold on the same title.
* The item is non-circulating.
* The item has no active copies.
* The member's account is not active.

### View Hold Details

To view the details of a specific hold:

* Go to `Dashboard -> Circulations -> Hold Queue`.
* Click on the `View` icon (eye) next to the hold you want to view.
* The hold detail page will display all information including member details, item details, hold type, queue position, status, and dates.

### Hold Actions

Staff can perform the following actions on holds from the hold queue list or detail page:

**Suspend a Hold**

To temporarily pause a hold:

* Click on the `Suspend` icon (pause) next to the hold.
* A modal will appear with a date picker.
* Select the date until which the hold should be suspended.
* Click `Submit` to suspend the hold.

The hold will maintain its queue position but will be skipped during fulfillment until the suspension date passes. Suspended holds are automatically reactivated when the suspension date arrives.

**Activate a Hold**

To reactivate a suspended hold before the suspension date:

* Click on the `Activate` icon (play) next to the suspended hold.
* The hold will change back to **Waiting** status and rejoin the active queue.

**Cancel a Hold**

To cancel a hold:

* Click on the `Cancel` icon (trash) next to the hold.
* A confirmation prompt will appear.
* Confirm the cancellation.

The hold will be cancelled, and queue positions will be recalculated for remaining holds. The member will receive a cancellation notification.

### Mark Ready

When a copy becomes available and needs to be manually assigned to a waiting hold:

* Go to the hold detail page.
* Click on the `Mark Ready` button.
* If multiple copies are available, select the copy to assign.
* The hold status will change to **Ready** and a pickup deadline will be calculated based on your Pickup Window setting.

**Note:** When the Fulfillment Mode is set to **Auto Assign**, holds are automatically marked as ready when an item is returned (checked in). Manual marking is needed when using **Staff Manual** mode, or when you want to override the automatic process.

---

## Hold Shelf

The hold shelf shows all holds that are in **Ready** status -- meaning the item has been set aside and is waiting for the member to pick it up.

To access the hold shelf:

* Go to `Dashboard -> Circulations -> Hold Queue -> Hold Shelf`.
* Ready holds will be displayed sorted by pickup deadline.
* Items are color-coded based on urgency:
	* **Red** -- Pickup deadline has passed (overdue).
	* **Yellow** -- Pickup deadline is within 2 days (expiring soon).
	* **Normal** -- Pickup deadline is more than 2 days away.
* Member contact information is displayed for easy communication.
* Click `Checkout` to fulfill the hold and issue the item to the member.
* Click `Cancel` to cancel the hold if the member does not pick up the item.

**Note:** Ready holds that pass their pickup deadline will be automatically expired by the system, and the item will be offered to the next member in the queue.

---

## Fulfill Hold (Checkout)

When a member comes to pick up a ready hold:

* Go to the Hold Shelf or the hold detail page.
* Click the `Checkout` button next to the ready hold.
* You will be redirected to the checkout form with the member and item pre-filled.
* Complete the checkout as usual.
* The hold status will change to **Fulfilled**.

Alternatively, you can check out items through the regular checkout process. If the item being checked out has an active hold for the member, the hold will be automatically fulfilled.

---

## Hold Demand

The hold demand page helps you identify high-demand items in your collection, which is useful for collection development decisions.

To view hold demand:

* Go to `Dashboard -> Circulations -> Hold Queue -> Hold Demand`.
* The top 50 high-demand items will be displayed.
* The following information is shown for each item:
	* **Title** -- The item title.
	* **Call No** -- The call number.
	* **Active Holds** -- Number of active holds on the item.
	* **Total Copies** -- Total number of copies in the collection.
	* **Available** -- Number of copies currently available.
	* **Ratio** -- Hold-to-copy ratio indicating demand level.
* Ratio is color-coded:
	* **Red** -- Ratio of 3 or higher (very high demand).
	* **Yellow** -- Ratio of 2 or higher (high demand).

Use this information to decide whether to purchase additional copies of high-demand titles.

---

## My Holds (Member Self-Service)

Members can place and manage their own holds from the catalog and their account area.

### Place Hold from Catalog

Members can place holds on items from the catalog detail page:

* Search for the item in the catalog.
* Click on the item title to view its details.
* If all copies are currently checked out, a `Place Hold` button will be displayed at the title level.

* Click the `Place Hold` button.
* A hold form will appear. If copy-level holds are enabled and multiple copies exist, you can select a specific copy.
* Add any notes if needed.
* Click `Submit` to place the hold.
* A success message will appear with your queue position.

Additionally, if copy-level holds are enabled, a `Hold` button will appear next to each individual copy that is currently checked out in the copies table.

**Note:** The `Place Hold` button is only visible when:

* The hold queue feature is enabled for the library.
* You are logged in as a member.
* Your member type matches the allowed member type setting (All, Regular, or Privileged).
* The item is a circulating item.
* Title-level holds are enabled (for the title-level button).
* All copies are currently checked out (for the title-level button), or the specific copy is checked out (for copy-level buttons).

If available copies exist, a message will be shown indicating that a hold is not needed since copies are available.

### View My Holds

To view your active holds:

* Click on `My Account` from the top menu.
* Click on `My Holds` to view your hold list.
* Each hold displays:
	* **Title** -- The item title.
	* **Hold Type** -- Title-level or Copy-level.
	* **Queue Position** -- Your position in the queue.
	* **Status** -- Current status with color-coded badge:
		* **Blue (Waiting)** -- Waiting for a copy to become available.
		* **Green (Ready)** -- Item is ready for pickup.
		* **Yellow (Suspended)** -- Hold is temporarily paused.
	* **Pickup Deadline** -- Displayed for Ready holds, showing the date by which you must pick up the item.

**Note:** My Holds only shows your active holds (Waiting, Ready, and Suspended). Fulfilled, Expired, and Cancelled holds are not displayed here.

### Suspend, Activate, and Cancel Holds

From the My Holds page, members can manage their holds:

**Suspend a Hold**

* Click the `Suspend` button next to a Waiting hold.
* Select the date until which you want to pause the hold.
* Click `Submit`.
* Your hold will be paused but your queue position will be maintained.

**Activate a Hold**

* Click the `Activate` button next to a Suspended hold.
* The hold will return to Waiting status and you can also activate it before the suspension date.

**Cancel a Hold**

* Click the `Cancel` button next to the hold.
* Confirm the cancellation.
* The hold will be cancelled and removed from the queue.

---

## How Hold Queue Works

### Hold Statuses

| Status | Description |
|--------|-------------|
| **Waiting** | Hold has been placed. Waiting for a copy to become available. |
| **Ready** | A copy has been assigned and is ready for pickup. Member must pick up within the Pickup Window. |
| **Fulfilled** | Member has picked up the item (checked out). The hold is complete. |
| **Expired** | Hold was not fulfilled before the expiration date (for Waiting holds) or the pickup deadline (for Ready holds). |
| **Cancelled** | Hold was cancelled by the member or staff. |
| **Suspended** | Hold is temporarily paused. It maintains its queue position but is skipped during fulfillment. |

### Hold Types

| Type | Description |
|------|-------------|
| **Title-level** | The member is waiting for any available copy of the item. When any copy is returned, it will be assigned to this hold. |
| **Copy-level** | The member is waiting for a specific copy. Only that particular copy will fulfill this hold. |

### Queue Positions (FIFO)

Holds are managed using a first-in, first-out (FIFO) queue:

* The first member to place a hold gets queue position 1.
* Each subsequent hold gets the next position in the queue.
* When a hold is cancelled or fulfilled, queue positions are recalculated automatically.
* Suspended holds maintain their queue position but are skipped during fulfillment.
* A member cannot place duplicate holds on the same title.

### Hold Fulfillment Flow

1. **Member or staff places a hold** -- A queue position is assigned. If **Auto-ready on placement** is enabled and a copy is currently available, the hold is immediately marked as Ready.
2. **Item is returned (checked in)** -- The system automatically checks for waiting holds on the returned item.
3. **Hold marked as Ready** -- The first eligible Waiting hold in the queue is assigned the returned copy, and a pickup deadline is calculated based on the Pickup Window setting.
4. **Member notified** -- If "Notify when hold is ready" is enabled, the member receives an email with the item title, accession number, and pickup deadline.
5. **Member picks up item** -- Staff checks out the item to the member, and the hold is marked as Fulfilled.
6. **If pickup deadline passes** -- The hold expires automatically, and the item is offered to the next member in the queue.

### Fulfillment Modes

The system supports three fulfillment modes that control what happens when a checked-out item is returned:

| Mode | Behavior |
|------|----------|
| **Auto Assign** | The returned item is automatically assigned to the next waiting hold. The hold is marked as Ready and the member is notified. This is the default and recommended mode. |
| **Notify & Confirm** | The member is notified that a copy is available and must confirm before the item is assigned to their hold. |
| **Staff Manual** | Staff must manually assign returned items to waiting holds using the Mark Ready action. |

### Recall System

When enabled, the recall system helps speed up item availability:

* When the first hold is placed on a currently checked-out item, the system shortens the current borrower's due date based on the **Recall Period** setting.
* The current borrower receives a recall notification informing them of the shortened return date.
* This encourages earlier return of high-demand items.

**Note:** Recall is triggered only when the **first** hold is placed on a checked-out item. Subsequent holds on the same item do not trigger additional recalls.

### Automatic Processing

The system runs automated background tasks to manage the hold queue:

* **Expired holds** -- Waiting holds that exceed the Hold Expiration days and Ready holds that exceed the Pickup Window are automatically marked as Expired.
* **Suspended holds** -- Holds that have passed their suspension end date are automatically reactivated to Waiting status.
* **Queue reassignment** -- When a Ready hold expires, the system automatically offers the item to the next Waiting hold in the queue.

---

## Notifications

The hold queue system sends the following notifications:

| Notification | When Sent | Details |
|-------------|-----------|---------|
| **Hold Placed** | When a hold is successfully placed | Includes item title and queue position number. |
| **Hold Cancelled** | When a hold is cancelled | Includes item title. |
| **Hold Ready for Pickup** | When a hold becomes ready | Includes item title, accession number of the assigned copy, and pickup deadline. |
| **Item Recalled** | When a recall is triggered | Sent to the current borrower with the original and shortened return dates. |
| **Hold Expired** | When a hold expires (if enabled) | Includes item title. Controlled by the "Notify when hold expires" setting. |

Notifications are sent only to members who have a linked user account. If email delivery fails for any reason, the hold action itself will still complete successfully -- notification failures are logged but do not prevent hold operations.

---

## Integration with Reservations

The hold queue system works alongside the existing reservation system:

* Both features can be enabled simultaneously and operate independently.
* **Reservations take priority over holds** -- If a returned item has both an active reservation and a waiting hold, the reservation will be fulfilled first.
* Holds will wait until any active reservations on the item are cleared before being processed.

For information on the reservation system, see the [Reserve Item](circulations.md#reserve-item) section in the Circulations page and the [Submit Reservation Request](member-area.md#submit-reservation-request) section in the Member Area page.
