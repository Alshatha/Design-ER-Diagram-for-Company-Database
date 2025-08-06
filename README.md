Entity-Relationship (ER) Diagram Design
This task involves designing an Entity-Relationship (ER) diagram to model the structure and rules of a company's employee–project–department system. The diagram visually represents the entities, attributes, relationships, and constraints involved in the system.

Key design elements include:

Entities and Attributes:
- Employee: SSN (PK), Fname, Lname, BirthDate, Gender
- Department: DNUM (PK), DName, Locations (multivalued)
- Project: PNumber (PK), PName, Location, City
- Dependent: DependentName (PK under Employee), Gender, BirthDate

Relationships and Constraints:
- Each employee is assigned to one department
- Each department can have multiple employees
- An employee may supervise other employees (recursive relationship)
- A department is managed by one employee, with HireDate stored in the relationship
- Each project belongs to one department but a department can have multiple projects
- Employees and projects have a many-to-many relationship with WorkingHours recorded
- An employee may have multiple dependents, tied by a weak entity relationship
- Dependents are deleted if the employee leaves

This ER diagram serves as a blueprint for the relational schema and database implementation.

📄 View the full solution here:
https://drive.google.com/file/d/1or5k3gkzVx9K83wy0gN_WJ29e34cdX5L/view?usp=sharing
