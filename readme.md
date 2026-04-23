# People That Own Pets ERM Assignment

## Theoretical Foundations

### 1. How are entities defined and represented in the ERM?
Entities are real-world objects, people, or concepts that store data in a database. They are usually represented as tables in modern ER diagrams.

Examples:
- People
- Pets

---

### 2. How are attributes defined and associated with entities?
Attributes are characteristics or details that describe an entity. They are represented as columns in a table.

Example:

People Table:
- person_id
- name
- email
- phone_number

---

### 3. What is a relationship in ERM, and how does it connect entities?
A relationship shows how two entities are connected.

Example:
A person owns a pet.

This connects the People table to the Pets table using a foreign key.

---

### 4. Cardinality Types

### One-to-One (1:1)
One record connects to only one other record.

Example:
One person → one passport

---

### One-to-Many (1:N)
One record connects to multiple records.

Example:
One person → many pets

---

### Many-to-Many (N:M)
Multiple records connect to multiple records.

Example:
Students can take many classes, and classes can have many students.

This usually requires a junction table.

---

# ERM Diagram: People That Own Pets

People
------
person_id (PK)
name
email
phone_number


Pets
------
pet_id (PK)
pet_name
breed
age
person_id (FK)


Relationship:
One Person → Many Pets
