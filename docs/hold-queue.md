# Hold queue

**Who this is for:** library staff, and members who place holds.

**What you can do here:** turn on holds, pull held books from the shelf, manage the queue and the hold shelf, and see how holds move from waiting to checkout.

The hold queue feature allows members to place holds on items that are checked out, and also on items that are on the shelf, and wait in a first-in, first-out (FIFO) queue. When a book on the shelf is held, staff take it from the shelf using [Holds to Pull](#holds-to-pull) and mark it ready. Library staff can manage the hold queue, hold shelf, and fulfil holds through the circulation dashboard. Members can also place and manage their own holds from the catalog and member area.

**Plans:** Hold queue is available on the **Basic Pro**, **Silver**, **Gold**, **Platinum** and **Unlimited** plans (see [What each plan includes](libraries.md#what-each-plan-includes)).

---

## Enable hold queue

To enable the hold queue feature for your library, please follow the below steps:

* Go to `Manage` > `Preferences`.
* Click on the `Hold Queue` tab.
* Check the `Enable hold queue` checkbox to activate the feature.
* Configure the hold queue settings as described below.
* Click on the `Save Preferences` button to save your changes.

### Hold queue settings

The following settings are available under the Hold Queue tab in Preferences:

| Setting | Description | Default |
|---------|-------------|---------|
| **Enable hold queue** | Master toggle to enable or disable the hold queue feature for your library. | Off |
| **Member** | Choose which member types can place holds: All Members, Regular Members Only, or Privileged Members Only. | All Members |
| **Hold Quota** | Maximum number of active holds a member can have at a time. | 5 |
| **Allow title-level holds** | Members can place holds on any available copy of a title. When a copy is returned, it will be automatically assigned. | On |
| **Allow copy-level holds** | Members can place holds on a specific copy of a title. | On |
| **Allow holds on items on the shelf** | Members can also hold items that are on the shelf. Staff take the copy from the shelf using Holds to Pull and mark it ready, and the member is told it is ready for pickup. When off, members can hold only items with every copy checked out. | On |
| **Hold Expiration** | Number of days before an unfulfilled hold expires automatically. | 180 |
| **Pickup Window** | Number of days a member has to pick up an item after it becomes ready. The same number of days is how long a copy on the shelf is kept for a waiting hold before it shows as **Overdue to pull** (see [When a copy is kept for a hold](#when-a-copy-is-kept-for-a-hold)). | 7 |
| **Fulfillment Mode** | How holds are fulfilled when items are returned. **Auto Assign:** A returned item is set aside for the next waiting hold, which becomes ready for pickup. **Staff Manual:** Returned items are not set aside. Staff choose which hold gets an item with Mark Ready on the Holds page. | Auto Assign |
| **Auto-ready on placement** | When staff place a hold and a copy is on the shelf, mark it ready at once (staff have the book in hand). Holds that members place themselves always wait in [Holds to Pull](#holds-to-pull) until staff press `Mark Ready`. | Off |
| **Enable recall** | When a hold is placed, shorten the due date for the current borrower to encourage earlier return. | Off |
| **Recall Period** | Number of days the current borrower has after a recall is triggered. | 7 |
| **Notify when hold is ready** | Send an email notification to the member when their hold is ready for pickup. | On |
| **Notify when hold expires** | Send an email notification to the member when their hold expires. | On |

---

## Hold queue (staff)

Library staff can manage all hold-related activities from the Hold Queue section in the Circulations menu.

### View hold queue

To view and manage all holds in your library:

* Go to `Circulations` > `Hold Queue`.
* The hold queue list will be displayed with all active holds.
* Use the status dropdown to filter holds by status: **Active**, **Actionable**, **Waiting**, **Ready**, **Suspended**, **Fulfilled**, **Expired**, **Cancelled**, or **All**.
	* **Active** (the default) -- Waiting, Ready and Suspended holds.
	* **Actionable** -- Waiting holds for titles that have a copy on the shelf right now, so you can mark them ready.
* Use the search box to find holds by title, ISBN, member name, or member number.
* The `Holds to Pull` button shows how many holds are waiting for a copy to be taken from the shelf (see [Holds to Pull](#holds-to-pull)). If some are overdue to pull, the page also says how many.

**Note:** If the hold queue feature is disabled, a warning message will be displayed with a link to the settings page.

### Place hold (staff)

Staff can place holds on behalf of members. To place a hold:

* Go to `Circulations` > `Hold Queue`.
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

If **Auto-ready on placement** is on and a copy is on the shelf, the hold is ready at once: *"Hold placed and immediately ready for pickup: put copy … on the hold shelf."* Otherwise a hold on a book that is on the shelf appears in [Holds to Pull](#holds-to-pull).

**Note:** The system will prevent placing a hold if:

* The member has reached their hold quota limit.
* The member already has an active hold on the same title.
* The item is non-circulating.
* The item has no active copies.
* The member's account is not active.

### View hold details

To view the details of a specific hold:

* Go to `Circulations` > `Hold Queue`.
* Click on the `View` icon (eye) next to the hold you want to view.
* The hold detail page will display all information including member details, item details, hold type, queue position, status, and dates.

### Hold actions

Staff can perform the following actions on holds from the hold queue list or detail page:

**Suspend a Hold**

To temporarily pause a hold:

* Click on the `Suspend` icon (pause) next to the hold.
* A modal will appear with a date picker.
* Select the date until which the hold should be suspended.
* Click `Submit` to suspend the hold.

The hold will maintain its queue position but will be skipped during fulfilment until the suspension date passes. Suspended holds are automatically reactivated on the day after the suspension date.

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

### Mark ready

When a copy is available and needs to be assigned to a waiting hold:

* Click `Mark Ready` on the hold detail page, in the hold queue list, or in [Holds to Pull](#holds-to-pull).
* If multiple copies are available, select the copy to assign.
* The hold status will change to **Ready** and a pickup deadline will be calculated based on your Pickup Window setting. The member is told the item is ready for pickup (if **Notify when hold is ready** is on).

**Note:** When **Fulfillment Mode** is set to **Auto Assign**, holds are automatically marked as ready when an item is returned (checked in). Manual marking is needed for holds on books that are on the shelf, when using **Staff Manual** mode, or when you want to override the automatic process.

---

## Holds to Pull

Holds to Pull lists the holds that a copy on the shelf can fill now, so staff can take the copy from the shelf and set it aside for the member.

* Go to `Circulations` > `Hold Queue` and click `Holds to Pull`.
* Each row shows when the hold was **Placed**, the **Title**, the **Copy on the shelf** (accession number and call number), the **Member** and the **Branch** of the copy. Holds that are overdue to pull are listed first.
* Take the copy from the shelf.
* Click `Mark Ready`. The **Mark Ready** window opens with that copy chosen. If the copy isn't on the shelf after all, choose another copy or leave the hold waiting.
* Click `Submit`. The hold becomes **Ready**, moves to the [Hold shelf](#hold-shelf), and the member is told it is ready for pickup.

A hold that is not pulled within your **Pickup Window** (counted from the day a copy on the shelf could first fill it) shows **Overdue to pull**. Other members may then borrow the copy from the shelf; the hold keeps its place in the queue and stays in the list while a copy on the shelf can fill it.

If you prefer members to borrow books from the shelf themselves, turn off **Allow holds on items on the shelf** in the `Hold Queue` tab of Preferences. Members can then hold only items with every copy checked out. Staff can still place holds on books on the shelf.

---

## Check in an item someone is waiting for

When you check in an item (see [Check-in item](circulations.md#check-in-item)) that has waiting holds, the message ends with one of these:

* **Hold assigned to next patron.** -- don't put the item back on the shelf. Put it on the hold shelf; it now appears in [Hold shelf](#hold-shelf) for that member, who is notified if notifications are on.
* **N hold(s) remaining in queue.** -- other members are still waiting for this title. If the message doesn't also say **Hold assigned to next patron.** (for example with the **Staff Manual** fulfilment mode), the item wasn't set aside; use `Mark Ready` (see [Mark ready](#mark-ready)) to give it to a waiting member.

---

## Hold shelf

The hold shelf shows all holds that are in **Ready** status -- meaning the item has been set aside and is waiting for the member to pick it up.

To access the hold shelf:

* Go to `Circulations` > `Hold Queue` and click `Hold Shelf`.
* Ready holds will be displayed sorted by pickup deadline.
* Items are colour-coded based on urgency:
	* **Red** -- Pickup deadline has passed (overdue).
	* **Yellow** -- Pickup deadline is within 2 days (expiring soon).
	* **Normal** -- Pickup deadline is more than 2 days away.
* Member contact information is displayed for easy communication.
* Click `Checkout` to fulfil the hold and issue the item to the member.
* Click `Cancel` to cancel the hold if the member does not pick up the item.
* Click `Undo ready` if you marked a hold ready by mistake. After you confirm (*"Undo ready for … ? The hold goes back to waiting and copy … back on the shelf."*), the hold is **Waiting** again in its place in the queue, and the copy goes back on the shelf. `Undo ready` is also on the hold detail page.

**Note:** Ready holds that pass their pickup deadline will be automatically expired by the system, and the item will be offered to the next member in the queue.

---

<a id="fulfill-hold-checkout"></a>

## Fulfil a hold (checkout)

When a member comes to pick up a ready hold:

* Go to the Hold Shelf or the hold detail page.
* Click the `Checkout` button next to the ready hold.
* You will be redirected to the checkout form with the member and item pre-filled.
* Complete the checkout as usual.
* The hold status will change to **Fulfilled**.

Alternatively, you can check out items through the regular checkout process. If the item being checked out has an active hold for the member, the hold will be automatically fulfilled. If the member's ready hold had set aside a different copy of the same title, the hold is fulfilled with the copy they borrow, and the copy that was set aside goes to the next member waiting.

---

## When a copy is kept for a hold

The same rules apply to staff checkouts, member self-checkouts and kiosks (only when **Enable hold queue** is on):

* A **Ready** hold keeps its copy for its member.
* **Waiting** holds keep a copy on the shelf only when there are not enough copies on the shelf for the members ahead in the queue. If there are enough, anyone can borrow the remaining copies.
* A waiting hold keeps a copy on the shelf for your **Pickup Window**, counted from the day a copy could first fill it. After that it shows **Overdue to pull** in [Holds to Pull](#holds-to-pull) and no longer stops others borrowing the copy. It keeps its place in the queue.
* Suspended holds don't keep copies.

Staff see a warning and can confirm to check the copy out anyway. Members and kiosks can't: a member sees *"This item is on hold for another member."* If staff check out a hold-shelf copy to someone else, the other member's hold goes back to **Waiting** in its place in the queue, or takes the copy that the borrower's own ready hold had set aside.

A loan is not renewed while another member is waiting for the item and the copies on the shelf can't serve them: see [Renew a loan](circulations.md#renew-a-loan).

---

## Hold demand

The hold demand page helps you identify high-demand items in your collection, which is useful for collection development decisions.

To view hold demand:

* Go to `Circulations` > `Hold Queue` and click `Hold Demand`.
* The top 50 high-demand items will be displayed.
* The following information is shown for each item:
	* **Title** -- The item title.
	* **Call No** -- The call number.
	* **Active Holds** -- Number of active holds on the item.
	* **Total Copies** -- Total number of copies in the collection.
	* **Available** -- Number of copies currently available.
	* **Ratio** -- Hold-to-copy ratio indicating demand level.
* Ratio is colour-coded:
	* **Red** -- Ratio of 3 or higher (very high demand).
	* **Yellow** -- Ratio of 2 or higher (high demand).

Use this information to decide whether to purchase additional copies of high-demand titles.

---

## My holds (member self-service)

What members see and do (place a hold from the catalog, see their queue position, suspend, activate or cancel a hold) is described in [Member area: My holds](member-area.md#my-holds).

---

## How hold queue works

### Hold statuses

| Status | Description |
|--------|-------------|
| **Waiting** | Hold has been placed. Waiting for a copy to become available. |
| **Ready** | A copy has been assigned and is ready for pickup. Member must pick up within the Pickup Window. |
| **Fulfilled** | Member has picked up the item (checked out). The hold is complete. |
| **Expired** | Hold was not fulfilled before the expiration date (for Waiting holds) or the pickup deadline (for Ready holds). |
| **Cancelled** | Hold was cancelled by the member or staff. |
| **Suspended** | Hold is temporarily paused. It maintains its queue position but is skipped during fulfilment. |

### Hold types

| Type | Description |
|------|-------------|
| **Title-level** | The member is waiting for any available copy of the item. When any copy is returned, it will be assigned to this hold. |
| **Copy-level** | The member is waiting for a specific copy. Only that particular copy will fulfil this hold. |

### Queue positions (FIFO)

Holds are managed using a first-in, first-out (FIFO) queue:

* The first member to place a hold gets queue position 1.
* Each subsequent hold gets the next position in the queue.
* When a hold is cancelled or fulfilled, queue positions are recalculated automatically.
* Suspended holds maintain their queue position but are skipped during fulfilment.
* A member cannot place duplicate holds on the same title.

<a id="hold-fulfillment-flow"></a>

### Hold fulfilment flow

1. **Member or staff places a hold** -- A queue position is assigned. If a copy is on the shelf, the hold appears in [Holds to Pull](#holds-to-pull) until staff mark it ready. If staff placed the hold and **Auto-ready on placement** is on, it is marked Ready at once.
2. **Item is returned (checked in)** -- The system automatically checks for waiting holds on the returned item.
3. **Hold marked as Ready** -- The first eligible Waiting hold in the queue is assigned the returned copy, and a pickup deadline is calculated based on the Pickup Window setting.
4. **Member notified** -- If "Notify when hold is ready" is enabled, the member receives an email with the item title, accession number, and pickup deadline.
5. **Member picks up item** -- Staff checks out the item to the member, and the hold is marked as Fulfilled.
6. **If pickup deadline passes** -- The hold expires automatically, and the item is offered to the next member in the queue.

<a id="fulfillment-modes"></a>

### Fulfilment modes

The system supports two fulfilment modes that control what happens when a checked-out item is returned:

| Mode | Behavior |
|------|----------|
| **Auto Assign** | The returned item is automatically assigned to the next waiting hold. The hold is marked as Ready and the member is notified. This is the default and recommended mode. |
| **Staff Manual** | Returned items are not set aside for holds. Staff choose which hold gets an item with the Mark Ready action on the Holds page. |

If you chose Notify & Confirm in the past, it now works as Auto Assign.

### Recall system

When enabled, the recall system helps speed up item availability:

* When the first hold is placed on a currently checked-out item, the system shortens the current borrower's due date based on the **Recall Period** setting.
* The current borrower receives a recall notification informing them of the shortened return date.
* This encourages earlier return of high-demand items.

**Note:** Recall is triggered only when the **first** hold is placed on a checked-out item. Subsequent holds on the same item do not trigger additional recalls.

### Automatic processing

The system runs automated background tasks to manage the hold queue:

* **Expired holds** -- Waiting holds that exceed the Hold Expiration days and Ready holds that exceed the Pickup Window are automatically marked as Expired.
* **Suspended holds** -- Holds are automatically reactivated to Waiting status on the day after their suspension end date.
* **Queue reassignment** -- When a Ready hold expires, the system automatically offers the item to the next Waiting hold in the queue.

---

## Notifications

The hold queue system sends the following notifications:

| Notification | When Sent | Details |
|-------------|-----------|---------|
| **Hold Placed** | When a hold is successfully placed | Includes item title and queue position number. |
| **Hold Cancelled** | When a hold is cancelled | Includes item title. |
| **Hold Ready for Pickup** | When a hold becomes ready | Includes item title, accession number of the assigned copy, and pickup deadline. When your library has more than one branch, it also names the branch where the copy is waiting. |
| **Item Recalled** | When a recall is triggered | Sent to the current borrower with the original and shortened return dates. |
| **Hold Expired** | When a hold expires (if enabled) | Includes item title. Controlled by the "Notify when hold expires" setting. |

Notifications are sent only to members who have a linked user account. If email delivery fails for any reason, the hold action itself will still complete successfully -- notification failures are logged but do not prevent hold operations.

---

## Integration with reservations

The hold queue system works alongside the existing reservation system:

* Both features can be enabled simultaneously and operate independently.
* **Reservations take priority over holds** -- If a returned item has both an active reservation and a waiting hold, the reservation will be fulfilled first.
* Holds will wait until any active reservations on the item are cleared before being processed.

For information on the reservation system, see the [Reserve Item](circulations.md#reserve-item) section in the Circulations page and the [Submit Reservation Request](member-area.md#submit-reservation-request) section in the Member Area page.

---

## FAQ

**Why is there no `Place Hold` button when a copy is on the shelf?**

Your library has turned off **Allow holds on items on the shelf**. The catalog then shows *"A copy is on the shelf. You can borrow it now."* and the member can borrow that copy instead. When the setting is on (the default), members can hold a book on the shelf and staff pull it for them.

**A member placed a hold on a book on the shelf. Why isn't it ready?**

Holds that members place always wait until staff take the copy from the shelf. Find the hold in [Holds to Pull](#holds-to-pull), take the copy and click `Mark Ready`.

**I marked a hold ready by mistake. Can I undo it?**

Yes. Click `Undo ready` on the [Hold shelf](#hold-shelf) or on the hold detail page. The hold goes back to Waiting in its place in the queue, and the copy goes back on the shelf.

**Can a member place a hold on an item they already have checked out?**

No. Librarika refuses the hold with the message "Member already has this item checked out."

**Can a member have more than one hold on the same title?**

No. A member can have only one active hold (Waiting, Ready or Suspended) per title, whether it is a title-level or a copy-level hold.

**Do suspended holds count towards the Hold Quota?**

Yes. Waiting, Ready and Suspended holds all count towards the member's [Hold Quota](#hold-queue-settings). Cancel a hold you no longer need to free up a place.

**Can a Ready hold be suspended?**

No. Only holds in **Waiting** status can be suspended. If the member cannot collect a Ready item in time, staff can cancel the hold from the [Hold Shelf](#hold-shelf).

**I cancelled a hold by mistake. Can I undo it?**

No. A cancelled hold cannot be reactivated. Place a new hold instead. The new hold joins the end of the queue, so the member does not get their old position back.

**What if staff check out a hold-shelf item to a different member?**

Librarika shows a warning that the item is on the hold shelf for another member, and staff can choose to continue. If you continue, the other member's hold goes back to Waiting in its place in the queue (or takes the copy the borrower's own ready hold had set aside).

**Can a recall give the current borrower more time?**

No. A [recall](#recall-system) only makes the due date earlier. If the borrower's due date already falls within the Recall Period, it is left unchanged.
