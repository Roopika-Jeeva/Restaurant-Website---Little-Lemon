# Little Lemon - Django Restaurant Management Application

## Project Overview

**Little Lemon** is a restaurant management system developed using the Django web framework as part of the **Meta Backend Developer Professional Certificate** on Coursera. This project demonstrates key concepts in Django, such as user authentication, database handling, and template inheritance, while providing an interactive platform for managing a restaurant’s menu, reservations, and orders.

## Features

- **User Authentication**: Allows users to register, log in, and log out.
- **Menu Display**: Browse and view restaurant menu items.
- **Admin Panel**: Manage menu items, reservations, and more via the Django admin interface.
- **Reservation System**: Users can make table reservations directly on the platform.
- **Form Handling**: Forms and ModelForms used to collect user data, such as reservations.
- **Database**: The project uses SQLite as the default database for development.
![image](https://github.com/user-attachments/assets/1b27d804-8281-4c17-a50c-091e06ebc642)

![image](https://github.com/user-attachments/assets/11730d55-3f18-4460-a03f-92f55550ed55)

![image](https://github.com/user-attachments/assets/d527a245-aafc-4ad1-b62b-66e43b9d277b)

![image](https://github.com/user-attachments/assets/755ccc5c-94cc-46b0-867c-243868398b4e)


## Technologies Used

- **Django**: Python web framework for building the backend and managing database models.
- **HTML & CSS**: For the structure and styling of the frontend.
- **Bootstrap**: For a responsive, mobile-friendly UI.
- **SQLite**: Database for development purposes (default for Django projects).

## Installation and Setup

### Prerequisites

Make sure you have the following installed:
- **Python 3.x**
- **Django** (you can install it via pip if necessary)

### Installation Guide

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/little-lemon-project.git
   cd little-lemon-project
   ```

2. **Create and activate a virtual environment** (optional but recommended):
   - On macOS/Linux:
     ```bash
     python3 -m venv env
     source env/bin/activate
     ```
   - On Windows:
     ```bash
     python -m venv env
     env\Scripts\activate
     ```

3. **Install dependencies**:
   Install the required packages from the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply database migrations**:
   Initialize the database by running:
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser**:
   Set up a superuser for the admin panel:
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server**:
   Start the Django development server:
   ```bash
   python manage.py runserver
   ```

7. **Access the application**:
   - Go to `http://127.0.0.1:8000/` to see the homepage.
   - Access the admin panel at `http://127.0.0.1:8000/admin` using your superuser credentials.

## Usage

- **View Menu**: Browse the available menu items on the homepage.
- **Make a Reservation**: Users can make table reservations through a simple form.
- **Admin Functionality**: Administrators can add, update, or delete menu items and manage customer reservations through the Django admin panel.

## Project Structure

```
little-lemon/
│
├── little_lemon/         # Django project settings and configurations
├── restaurant/           # Main Django app containing views, models, and templates
│   ├── migrations/       # Database migration files
│   ├── models.py         # Database models (Menu, Reservation, etc.)
│   ├── views.py          # Views for handling web requests
│   ├── forms.py          # Forms and ModelForms for input handling
│   └── templates/        # HTML templates for rendering pages
├── static/               # Static files (CSS, JavaScript)
├── db.sqlite3            # SQLite database file
└── manage.py             # Command-line utility for Django
```

## Future Enhancements

- **Search Functionality**: Implement search and filter capabilities for the menu.
- **Order Management**: Add functionality for customers to place food orders.
- **Payment Gateway**: Integrate online payment options for reservations and orders.
- **API Integration**: Provide a REST API for mobile app integration or external services.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and submit a pull request.

For major changes, please open an issue first to discuss what you would like to modify.

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

