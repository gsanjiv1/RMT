# Django Project

This is a Django project with instructions on how to set it up and run it locally.

## Setup

1. Clone this repository to your local machine.

2. Navigate to the project directory:

    ```bash
    cd rmcmt
    ```

3. Create a virtual environment:

    ```bash
    python3 -m venv env
    ```

4. Activate the virtual environment:

    - On Windows:

    ```bash
    .\env\Scripts\activate
    ```

    - On macOS and Linux:

    ```bash
    source env/bin/activate
    ```

5. Install the project dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Running the Project

1. Navigate to the Django project directory.

2. Apply migrations:

    ```bash
    python manage.py migrate
    ```

3. Create a superuser (optional):

    ```bash
    python manage.py createsuperuser
    ```

4. Load Initial Datas:
    Load data in order:

    ```bash
    python manage.py loaddata fixtures/initial_question_type.json

    python manage.py loaddata fixtures/initial_risk_scale.json

    python manage.py loaddata fixtures/initial_questions.json

    python manage.py loaddata fixtures/initial_answers.json
    ```

5. Start the development server:

    ```bash
    python manage.py runserver
    ```

5. Open a web browser and go to `http://127.0.0.1:8000/` to view the application.

6. To access the Django admin interface, go to `http://127.0.0.1:8000/admin/` and log in with the superuser credentials created in step 3.


