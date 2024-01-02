
# Registration module

Hyperlambda registration module for Magic, giving you workflow actions for easily creating registration
and user management logic. The following actions are included in the module.

* extras-get - Retrieves extra information for users, such as email and name
* extras-remove - Removes extra information associated with users
* extras-upsert - Inserts or updates extra information associated with users
* roles-add - Adds the specified role to some user
* roles-get - Returns all roles associated with user
* roles-remove - Removes the specified role from user
* username-available - Checks if a username is available to use for registering new users
* users-change-password - Changes the password for a specified user
* users-create - Creates a new user, allowing you to among other things create registration logic
* users-delete - Deletes a user entirely from the system
* users-get - Returns information associated with some user

By combining the above actions it should be fairly easy to create registration logic in Magic.
