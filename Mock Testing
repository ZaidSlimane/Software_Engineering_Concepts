# Mocking in Software Engineering

Mocking is the process of simulating the external dependencies of the code that's being tested. This allows you to isolate your code from the multitude of things it depends on, making testing simpler and more efficient. 

Mocking typically comes in two forms:
- **Fake Data**
- **Fake Interactions**

---

### Why Mocking is Useful?

Let's say you have a function that depends on an external service, like a database. Instead of actually connecting to a database (which may be slow, require setup, or introduce dependencies you don't want to test), you can **mock** the database connection.

#### Example: Database Connection Mocking

Consider the following function that queries a database:

```python
# Function to be tested
def get_user_name(user_id, db_connection):
    query = f"SELECT name FROM users WHERE id = {user_id}"
    result = db_connection.execute(query)
    return result.fetchone()[0]
