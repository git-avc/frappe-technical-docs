# Doctype Fields

In Frappe, Doctype (short for "Document Type") is a fundamental concept used to define the structure of documents or records in a database. A Doctype specifies the fields, data types, and behavior of a particular type of document or record. Fields within a Doctype represent the attributes or properties of the document, and they define what information can be stored in each document of that type. Here's an overview of Frappe Doctype fields:

1. **Field Types**: Frappe provides various field types to accommodate different types of data. Some common field types include:

   - Text: For short text data.
   - Long Text: For longer text data, such as descriptions or comments.
   - Integer: For whole numbers.
   - Float: For decimal numbers.
   - Date: For dates.
   - Date and Time: For date and time values.
   - Currency: For monetary values.
   - Check: For boolean (true/false) values.
   - Select: For predefined options in a dropdown.
   - Link: For linking to other Doctypes or records.
   - Table: For creating a table of related records within a document.

2. **Field Labels**: Each field in a Doctype has a label that describes what the field represents. For example, a "Name" field might have the label "Full Name."

3. **Field Names**: Field names are used to identify fields programmatically. They are often in lowercase and may contain underscores (e.g., "full_name").

4. **Mandatory Fields**: You can mark fields as mandatory, indicating that they must be filled in before a document of that type can be saved.

5. **Read-only Fields**: Read-only fields are fields that users can view but cannot edit. They are often used for calculated or system-generated data.

6. **Hidden Fields**: Hidden fields are not displayed on the user interface but can be used to store data or perform calculations behind the scenes.

7. **Default Values**: Fields can have default values, which are automatically filled in when a new document is created.

8. **Dependent Fields**: The visibility or value of a field can depend on the value of another field. For example, a "Shipping Address" field might only be visible if a "Use Different Shipping Address" checkbox is checked.

9. **Field Permissions**: Field-level permissions can be set to control who can view or edit specific fields within a document.

10. **Validation**: You can define validation rules for fields to ensure that data entered meets specific criteria. For example, a field can be required to contain an email address format.

11. **Options**: For fields like "Select," you can define a list of predefined options that users can choose from in a dropdown menu.

12. **Link Fields**: Link fields are used to create relationships between Doctypes. For example, a "Customer" field in a sales order might link to a customer record.

13. **Table Fields**: Table fields allow you to create tables of related data within a document. Each row in the table corresponds to a related record.

14. **Custom Fields**: You can create custom fields in addition to the standard fields provided by Frappe. Custom fields can be of various types and used to store additional data specific to your application.

15. **Scripts**: Field behavior can be customized using JavaScript scripts. Scripts can be used to perform actions like field calculations, data validation, and dynamic updates.

Frappe Doctype fields are essential for defining the structure and functionality of documents in your application. They determine how data is captured, displayed, and processed within the system, making them a central aspect of designing and customizing applications built on the Frappe framework.
