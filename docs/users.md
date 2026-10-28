# Users

Users are those who can administer or manage all the activities of your library depending on their role. They can sign in to the library dashboard and do regular managerial activities. They can also add or remove a user from the library.

**Users vs Members:** Users and Members are different concepts in Librarika. Users are staff accounts with access to the library dashboard for managerial activities. Members are library-specific records for people who borrow items. A person can be both a user and a member. For more details on members, see the [Members](members.md) page.

**Editing user information:** User accounts are independent and can be linked to multiple libraries across the Librarika platform. As a library admin, you can change a user's role and permissions, but you cannot directly edit their personal details (name, email, etc.). Users manage their own personal information through their Account Settings by clicking on their profile icon.

## List users

Users is the section where you can see all the list of users based on their roles. They have access to the library and can do all the regular managerial workings of the library. 

To view list admin or stuff users, please follow the below steps:

* First, sign in to your library.
* Please go to the `Dashboard ->  Manage -> Users` dropdown menu.

	![Users dropdown menu](img/user-dropdown-menu.png)

* Click on `Users` and a page will be appeared like below. Here you can see all the users of your library.

	![Users main page](img/users-main-page.png)

* If you click on the `View` icon next to any user then you can see all the information of that specific user like below.

	![Users user view page](img/users-view-page.png)

* Here you can also see the group information of that user, if you click on the view icon from the **Group Memberships** table.

	![Users view group info](img/users-group-info.png)

* Now you can also view all the related members of that group.

### Last active

The **Last active** column shows when each user last signed in to your library or opened it in the Librarika app.

![Users list with the Last active column](img/users-last-active-column.png)

* A dash (`—`) means the user hasn't signed in to your library since this was introduced.
* Only their own sign-ins count. A visit by Librarika support never does.
* You can't see a user's sign-in history, devices or addresses. Each user sees their own in [Sign-in activity](sign-in-activity.md#sign-in-activity).


## Add user

User with library admin privileges can add a new user and give them access to the library for managerial activities.

To add a user, please follow the below steps:

* Please go to the `Users` section from the `Manage` dropdown menu.
* Click on `New User` button and a create user form will be appeared like below.

	![Users add user form](img/users-add-user-form.png)

* Enter the user's **Email** and tick one or more **Groups / Roles**:
	* **Library Administrator** -- full access to all library settings and management features, including users, preferences and sign-in security.
	* **Library Assistant** and **Library Staff** -- day-to-day library work such as circulation and cataloging. The form links to the **Librarika Permissions** page, which lists what each role can do.
* If the email doesn't belong to a Librarika account yet, a **Name** field appears. Enter the person's name.

	![Users add user form name field](img/users-add-user-form-name-field.png)

* **Employee** (optional): link an employee profile from **Others** > **Employees** to this account.

* Click on `Submit` button and a user will be invited to join your library and the status for this new user will be **Invited**.

	![Users main page](img/user-with-invited-status.png)

* Now the user needs to follow the invitation email and join the library. 


## Resend invitation

When you will create a new user an invitation email will automatically send to the users email account for joining your library. That time if the user can not join the library for some reason then you can send the joining request again by clicking on re-send invite option.  

To do so, please follow the below steps:

* Please go to the `Users` section.
* Locate that user whom you want to send the invitation email again from users section and click on the `Re-send Invite` button on the right to that user.

	![Users resend invite link](img/user-resend-invite-button.png)

* Click on it and the invitation email will be send to the users email account for joining your library.
* If an user click on the joining request, then that user will be able to join the library.
* Now the status of this new user will be turned into **Active** from **Invited**.


## Add / update permission

You can change the groups or roles of a user by setting permissions for the users.

To set permissions, please follow the below steps:

* Click on `Change Permissions` icon from the users section.
* A form will be appeared like below.

	![Users change permissions page](img/users-change-permissions-page.png)

	When your library can limit users to branches, the dialog also has a **Branch Access** section below the roles (not shown here; see [Branch access](#branch-access)).

* Here you can change the groups or roles of a user from the previous one by changing permissions. You can also add permission for a new user.
* Also you can select multiple groups or roles for a user when you will either add or update permission.
* Click on `Save` button when you are done and your permissions will be saved.

## Branch access

On plans that include branch access, and when your library has more than one branch, you can limit a user to some branches.

* Click `Change Permissions` for the user.
* Under **Branch Access**, untick **Full Access (All Branches)** and tick the branches they may work in (*"Restrict this user to specific branches. Leave "Full Access" checked for unrestricted access."*).
* Click `Save`.

The user then sees and changes only the copies, loans and holds of those branches, and the Users list shows **Branch Restricted** next to their name. Library Administrators always have every branch (*"Library Administrators always have full access to all branches."*). To give the user every branch again, tick **Full Access (All Branches)**.

The same **Branch Access** section is on a member's edit page, for members who use self-service.

## Remove permission

You can also remove the permissions that you have given to the users for your library.

To remove the permissions, please follow the below steps:

* Click on `Change Permissions` icon like before from the users section.
* Now the `Change Permissions` form will be appeared same as the **Add / Update Permission** section mentioned above.
* In the `Change Permissions` form you have to uncheck the gruops or roles options and click on **Save** button.

	![Users remove permissions page](img/users-remove-permissions-page.png)

* Now the permissions will be removed for the users.

## Linked members

Linked members is the section where you can see the list of users who have access to the members area section of your library. Basically they are the members or patrons with log in access.

To view the list of linked members, please follow the below steps:

* Click on `Switch to Linked Members` button from the top of the users section.

	![Users linked members button](img/users-linked-members-button.png)

* Now click on the switch to linked members button and the `Linked Members` page will be appeared like below.

	![Users linked members page](img/users-linked-members-page.png)

* All the member accounts are listed here. These users can not access admin dashboard by default. 
* However, you can assign them admin permission, if you want them to be a part of your library management staff.

---

## FAQ

**What does the Last active column show?**

When the user last signed in to your library or opened it in the Librarika app. See [Last Active](#last-active).

**Can I change a staff member's name, email or password?**

No. Each person manages their own account in their settings. You can change their role or remove their permission (see [Add / Update Permission](#add-update-permission) and [Remove Permission](#remove-permission)).

**An invited user didn't receive the email. What can I do?**

Use [Resend Invitation](#resend-invitation), and ask them to check their spam folder.

**Which password does an invited user choose?**

A new password for Librarika, separate from their email and their organisation's SSO password. The invitation page explains this. See [Your Librarika password and your organisation's password](signing-in.md#your-librarika-password-and-your-organisations-password).

**A staff member lost their phone. How do they sign it out?**

They open their [Sign-in activity](sign-in-activity.md#sign-in-activity) and click `Sign out` next to the phone, or change their password, which signs out every other session. If the phone had their authenticator app, they sign in with a recovery code and use `Set up a new phone`. See [Lost your phone?](two-step-verification.md#lost-your-phone).

**Can I turn off a staff member's two-step verification or reset their password?**

No. They reset their own password with `Forgot password?`. If they lost their phone and their recovery codes, they contact Librarika support, who can turn off two-step verification after checking who they are. See [Helping someone who can't sign in](helping-people-sign-in.md).

**Can I require two-step verification for staff?**

Yes, on the Gold plan and higher, in **Preferences** > `Sign-in security`. See [Sign-in security](library-sign-in-security.md).

**What does "Branch Restricted" mean in the Users list?**

The user can work only in some of your branches. See [Branch access](#branch-access).

**How do I stop someone from managing my library?**

Remove their permission (see [Remove Permission](#remove-permission)). Their Librarika account stays, but they can no longer open your library's dashboard.
