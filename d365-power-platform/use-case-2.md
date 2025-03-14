# Database Design

 The company wants to automate their order processing system. However, before automating anything, they need a well-structured database. You must design an Entity Relationship Diagram (ERD) and define the necessary tables, column, data types and relationship between the tables.

🔍 Your Task:

Identify Key Tables – Below are the necessary tables you must create:

Customers (CustomerID, Name, Email, Phone, Address)

Orders (OrderID, CustomerID, OrderDate, Status, TotalAmount)

Products (ProductID, Name, Description, Price, StockQuantity)

OrderDetails (OrderDetailID, OrderID, ProductID, Quantity, Subtotal)

Inventory (InventoryID, ProductID, WarehouseLocation, StockLevel)

Employees (EmployeeID, Name, Role, Department, Email)

Payments (PaymentID, OrderID, PaymentMethod, Amount, PaymentDate)

Understand Relationships:

Each Customer can place multiple Orders.

Each Order contains multiple Products (Many-to-Many relationship resolved via OrderDetails).

Products are stored in Inventory.

Each Order has a corresponding Payment.

Employees process Orders and handle customer service requests.

 ## Question:
 Design an Entity Relationship Diagram (ERD) connecting these tables.
