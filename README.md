# Little Lemon Restaurant Booking System

This project is a web-based booking system for the fictional "Little Lemon" restaurant. It allows users to make reservations by selecting a date and time and provides an overview of existing bookings. This project was developed as part of an assignment for the Meta Full Stack course on Coursera.

## Project Purpose

The primary goal of this project is to demonstrate the following skills and concepts learned in the Meta Full Stack course:

-   **Full-Stack Development:**  Building a complete web application that includes both front-end (user interface) and back-end (data handling and server logic) components.
-   **Database Integration:**  Using MySQL to store booking data, including data models, database schemas, and data persistence.
-   **Django Framework:** Employing Django for building the web application with Model-View-Template (MVT) architectural patterns.
-   **Form Handling:**  Creating and processing web forms to capture user input.
-   **AJAX Interactions:** Implementing AJAX for dynamic updates of web pages.
-   **JSON Data Handling:** Working with JSON for data exchange between the client-side and server-side.
-   **User Interface:** Creating a user-friendly interface using HTML, CSS, and basic JavaScript.
-   **API Design:** Creating an endpoint for making requests to retrieve and add data.

## Features

The application has the following features:

-   **Booking Form:**
    -   Allows users to select a date and time for a reservation.
    -   Displays available time slots.
    -   Disables already booked time slots.
    -   Automatically selects the current date.
    -   Displays bookings for the selected date under the form.
-   **Reservations Page:**
    - Displays the bookings.
    - Allows the user to select a date and filter all the bookings based on that date.
-  **Navigation:**
   -  A navigation bar that enables navigation between the main page, the booking page and the reservations page.

## Technologies Used

-   **Python:**  The core programming language for the back-end.
-   **Django:**  A high-level Python web framework for building the application.
-   **MySQL:**  The database system for storing booking data.
-   **HTML, CSS, JavaScript:**  Used for the front-end user interface.
-   **Pipenv:** Dependency management and virtual environment.

## Setup Instructions

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Abubakr-Alsheikh/little-lemon-backend-api.git
    cd little-lemon-backend-api
    ```

2.  **Set Up the Database:**
    -   Make sure you have a MySQL server running and have created a database named `reservations`.
    -   Create a user with appropriate privileges.

3.  **Set up the environment**
     ```bash
       pipenv install
       pipenv shell
     ```
4.  **Install Dependencies:**
    ```bash
    pipenv install django mysqlclient
    ```

5. **Update `settings.py`:**
    - Configure your Django application to use your database settings in the `settings.py` file.

6.  **Run Migrations:**
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

7.  **Run the Development Server:**
    ```bash
    python manage.py runserver
    ```

8.  **Access the Application:**
    - Open your web browser and go to `http://127.0.0.1:8000/`.

## Usage

1.  **Booking:**
    -   Navigate to the "Book" page.
    -   Fill in your name.
    - Select a date.
    -   Select a time from the dropdown.
    -  Click the "Reserve Now" button.
     - If the selected time is not available, an error will be shown.
   - The booking entries will appear below the form.

2.  **Viewing Reservations:**
    -   Navigate to the "Reservations" page.
   -    View all the entries for current day.
    -  Select a different date to view all the entries for that day.

## Learning Outcomes

By completing this project, the student should be able to:

-   Develop a full-stack web application from scratch using Django and MySQL.
-   Integrate database access with Django models and views.
-   Create and validate web forms.
-   Use AJAX for dynamic updates of web pages.
-   Work with JSON for data transfer.
-   Implement a basic REST API endpoint.

## Additional Notes

This project is a demonstration of the concepts taught in the Meta Full Stack course. In a real-world scenario, more features and robust validation, such as payment, user authentication, and detailed error handling, would be included.

## License

This project is not licensed at the moment and is for demonstrational purposes only.