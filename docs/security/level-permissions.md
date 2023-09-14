# Module Level Permissions
Frappe allows you to assign permissions at the module level. For example, you can grant the "Sales Manager" role permission to access the "Sales" module but restrict access to the "HR" module.

# DocType-Level Permissions
Permissions can be further refined by specifying which DocTypes (database tables) users with a specific role can access and what actions they can perform. For instance, the "HR Manager" role might have full access to the "Employee" DocType, allowing them to create, read, update, and delete records.

    When you enter 0 is to access the application (Module) any higher level is dedicated to the field level permissions.

# Field-Level Permissions
Within a DocType, you can set field-level permissions. This allows you to control which fields users with a particular role can see and edit. For example, you can hide sensitive information from certain roles.

# Permission Manager
Frappe provides a user-friendly "Permissions Manager" where administrators can set and configure role-based permissions. This interface simplifies the process of granting and revoking access rights to various modules and DocTypes.