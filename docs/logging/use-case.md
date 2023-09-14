# Use Case Scenario

Consider the following scenario: you've created an API that will update a counter with the value supplied by the user and return the updated number. You should now log data in the API to ensure that everything is operating properly. As a result, you develop a logger API to track events for the same.

# Implementation

```python
frappe.utils.logger.set_log_level("DEBUG")
logger = frappe.logger("api", allow_site=True, file_count=50)


@frappe.whitelist()
def update(value):
    user = frappe.session.user
    logger.info(f"{user} accessed counter_app.update with value={value}")

    current_value = frappe.get_single_value("Value", "counter")
    updated_value = current_value + value
    logger.debug(f"{current_value} + {value} = {updated_value}")
    frappe.db.set_value("Value", "Value", "counter", updated_value)
    logger.info(f"{user} updated value to {value}")

    return updated_value

```