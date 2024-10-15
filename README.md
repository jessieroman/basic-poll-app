# Polls App

A simple polling application built with Django, demonstrating CRUD operations, user interaction, and admin management. This project showcases my ability to develop web applications using the Django framework, following best practices and efficient coding standards.

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Key Learnings](#key-learnings)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)

## Features

- **Create Polls:** Users can create new polls with multiple choices.
- **Vote:** Users can vote on their preferred options.
- **Results Display:** Real-time display of poll results.
- **Admin Interface:** Manage polls and choices through Django’s admin panel.
- **User Authentication:** Secure user login and registration (if implemented).
- **Responsive Design:** Mobile-friendly interface for accessibility.

## Technologies Used

- **Backend:** Django 5.1
- **Frontend:** HTML, CSS, JavaScript
- **Database:** SQLite (default for Django projects)
- **Version Control:** Git, GitHub
- **Others:** Bootstrap (if used for styling), Django REST Framework (if applicable)

## Installation

Follow these steps to set up the Polls App locally:

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/polls-app.git
    cd polls-app
    ```

2. **Create a Virtual Environment:**

    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    ```

3. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply Migrations:**

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5. **Create a Superuser:**

    ```bash
    python manage.py createsuperuser
    ```

6. **Run the Development Server:**

    ```bash
    python manage.py runserver
    ```

7. **Access the Application:**
    - Open your browser and navigate to `http://127.0.0.1:8000/polls/`
    - Access the admin panel at `http://127.0.0.1:8000/admin/`

## Usage

1. **Viewing Polls:**
    - Navigate to the polls section to view all available polls.
    - Click on a poll to see its details and voting options.

2. **Voting:**
    - Select your preferred choice and submit your vote.
    - After voting, you’ll be redirected to the results page displaying current poll standings.

3. **Admin Management:**
    - Log in to the admin panel using your superuser credentials.
    - Create, update, or delete polls and choices as needed.

![Polls List](screenshots/polls_list.png)
![Poll Detail](screenshots/poll_detail.png)
![Admin Panel](screenshots/admin_panel.png)

## Project Structure

## Key Learnings

- **Django Framework:** Gained hands-on experience with Django’s MVC (Model-View-Controller) architecture.
- **CRUD Operations:** Implemented Create, Read, Update, and Delete functionalities.
- **URL Routing:** Mastered mapping URLs to views and using namespaces to avoid conflicts.
- **Template Rendering:** Utilized Django’s templating system to create dynamic HTML pages.
- **Admin Customization:** Configured the Django admin interface for efficient data management.
- **Form Handling:** Managed user input securely with form validation and CSRF protection.
- **Version Control:** Effectively used Git for version tracking and collaboration.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- **Django Documentation:** [https://docs.djangoproject.com/en/5.1/intro/tutorial04/](https://docs.djangoproject.com/en/5.1/intro/tutorial04/)
- **Choose a License:** [https://choosealicense.com/](https://choosealicense.com/)
- **GitHub Guides:** [https://guides.github.com/](https://guides.github.com/)

## Future Improvements

- **User Authentication:** Implement user registration and login functionalities.
- **Enhanced UI/UX:** Improve the frontend with better design and responsiveness.
- **REST API:** Develop a RESTful API for the polls app.
- **Deployment:** Deploy the application to a cloud platform like Azure or AWS.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.
