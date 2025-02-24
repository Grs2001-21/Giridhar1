# Testing Strategy

## 1. Unit Tests
Approach:

> Unit tests focus on testing individual functions and business logic in isolation.
> External dependencies, such as MongoDB, are mocked using unittest.mock and mongomock.
> The tests follow the AAA (Arrange, Act, Assert) pattern for clarity and maintainability.
>Coverage is measured using pytest-cov.
### Run the following command
   pytest tests/unit --cov=app


## 2. Integration Tests
Approach:

> Integration tests check the API endpoints and simulate real user interactions.
>The tests use httpx.AsyncClient to make HTTP requests to the FastAPI application.
> A separate test database is used to avoid affecting real data.
> Tests cover major CRUD operations (Create, Read, Update, Delete).
### Run the following command
 pytest tests/integration --cov=app


## 3. Code Coverage
  Code coverage is tracked using pytest-cov.
### Run the following command to check the coverage:
   pytest --cov=app


# How to Set Up and Run Tests Locally
   ### Clone the repository
      git clone https://github.com/Grs2001-21/Giridhar1.git
      cd Giridhar1

   ### Create a virtual environment
      python -m venv venv

   ### Activate the virtual environment
   ### On Windows (Git Bash)
    source venv/Scripts/activate

   ### Install dependencies
    pip install -r requirements.txt

   ### Run tests
    pytest --disable-warnings --cov=app tests/


