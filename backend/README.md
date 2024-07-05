# Doom Library

Doom Library is a Flask-based web application to manage book loans. It provides functionalities to add, update, delete, and view books, as well as manage customer loans.

## Features

- Add new books to the library
- Update book information
- Delete books from the library
- View all books in the library
- Manage customer loans

## Requirements

- Python 3.8+
- Flask
- Flask-SQLAlchemy
- Flask-CORS

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/doom-library.git
    cd doom-library
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up the database:
    ```bash
    flask db init
    flask db migrate -m "Initial migration."
    flask db upgrade
    ```

5. Run the application:
    ```bash
    flask run
    ```

## Usage

Open your web browser and go to `http://127.0.0.1:5000` to access the Doom Library application.

## API Endpoints

### Books

- `GET /books` - Retrieve all books
- `GET /books/<int:book_id>` - Retrieve a specific book by ID
- `POST /add_book` - Add a new book
- `PUT /books/<int:book_id>` - Update an existing book
- `DELETE /books/<int:book_id>` - Delete a book

### Loans

- `GET /loans` - Retrieve all loans
- `GET /loans/<int:loan_id>` - Retrieve a specific loan by ID
- `POST /add_loan` - Add a new loan
- `PUT /loans/<int:loan_id>` - Update an existing loan
- `DELETE /loans/<int:loan_id>` - Delete a loan

## License

This project is licensed under the MIT License.
