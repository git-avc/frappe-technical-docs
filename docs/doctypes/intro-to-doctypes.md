# What is a Doctype?

In the Frappe framework, a "Doctype" (short for "Document Type") is a fundamental concept that represents a structured data model. Doctypes are used to define the structure of documents or data records in an application. They provide a way to specify the fields and relationships between those fields for storing and managing different types of information in a structured manner.

Here are some key points about Doctypes in Frappe:

1. **Structured Data Modeling**: Doctypes are used to define the structure of documents in a hierarchical and relational manner. Custom Doctypes are created to represent various data entities or objects within an application, such as customers, products, orders, invoices, and more.

2. **Fields**: Each Doctype consists of fields that define the attributes or properties of the document. Fields can represent different data types, such as _text_, _numbers_, _dates_, and _links_ to other documents.

3. **Relationships**: Doctypes can have relationships with other Doctypes. These relationships are defined using fields like _Link_ fields, which establish connections between different documents. For example, an "Order" Doctype may have a Link field to associate it with a "Customer" Doctype.

4. **Customization**: Doctypes can be entirely customized to match the specific data structure and business requirements of an application.

5. **Workflow**: Workflows can be defined for Doctypes, specifying the sequence of steps or states a document can go through. This is useful for modeling and automating business processes.

6. **Validation and Permissions**: Doctypes allow defining data validation rules and access permissions to control who can create, read, update, or delete documents of a particular Doctype.

7. **Scripting**: Server-side scripts (in Python) can be associated with Doctypes to add custom business logic, automate tasks, or trigger actions based on document events.

8. **User Interface**: Frappe's user interface (UI) framework is designed to work seamlessly with Doctypes, providing forms for creating and editing documents, as well as listing views for displaying collections of documents.

9. **REST API**: Each Doctype comes with a built-in RESTful API, making it easy to interact with and manipulate data programmatically.

10. **Reports and Dashboards**: Reports and dashboards can be generated based on data stored in Doctypes to gain insights into the application's data.

In short, Doctypes in Frappe provide a powerful and flexible way to _define_, _store_, and _manage_ structured data in frappe application.
