# Django GraphQL Library

This is a basic Django project that demonstrates how to set up a GraphQL API using Graphene-Django.

## Setup

### Requirements

- Python 3.x
- Django
- Graphene-Django

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. Create a virtual environment and activate it:

    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Apply migrations:

    ```bash
    python manage.py migrate
    ```

5. Create a superuser:

    ```bash
    python manage.py createsuperuser
    ```

6. Run the development server:

    ```bash
    python manage.py runserver
    ```

### Usage

To access the GraphQL interface, navigate to `http://127.0.0.1:8000/graphql/` in your web browser. You should see the GraphiQL interface where you can run queries.

### Example Query

To fetch all books, use the following query:

```graphql
{
  allBooks {
    id
    title
    excerpt
  }
}
