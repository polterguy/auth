
Auth module for Magic, giving you workflow actions for easily creating registration
and user management logic.

## Workflow actions

* authenticate - Authenticates the specified user and returns a JWT token
* authorize - Ensures user is authorized to access some resource
* extras-get - Retrieves extra information for users, such as email and name
* extras-remove - Removes extra information associated with users
* extras-upsert - Inserts or updates extra information associated with users
* roles-add - Adds the specified role to some user
* roles-get - Returns all roles associated with user
* roles-remove - Removes the specified role from user
* username-available - Checks if a username is available to use for registering new users
* username-get - Returns the username for the currently authenticated user
* users-change-password - Changes the password for a specified user
* users-create - Creates a new user, allowing you to among other things create registration logic
* users-delete - Deletes a user entirely from the system
* users-get - Returns information associated with some user

By combining the above actions it should be fairly easy to create registration logic in Magic.

## Workflows

In addition the module contains a reusable workflow encapsulating the imports actions from above, correctly
changed together. This workflow is as follows.

* register - Registers a new user with the specified username, password, email, and name - And optionally associated the user with a default role
