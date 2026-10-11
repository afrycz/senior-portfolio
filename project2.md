Student Registration System
===========================

- **Class:** CSCI 332
- **Grade:** A (course grade)
- **Language(s):** PHP, HTML, CSS
- **Source Code Repository:** [CSCI332-Student-Registration-System](https://github.com/afrycz/CSCI332-Student-Registration-System)

Project Description
-------------------

The Student Registration System is a web application that collects student registration information through a form, validates the submitted data, saves valid entries to a CSV file, and displays the saved registrations in a table.

The project uses PHP to process the submitted form data, HTML to build the pages, and CSS to control the layout and appearance.

How to Run the Program
----------------------

No compilation is required.

The project is run from a web server that supports PHP. For testing, PHP's built-in web server can be started from the project folder with:

```bash
php -S localhost:8000
```

Then open the registration page in a browser:

```text
http://localhost:8000/registration.php
```

How It Works
------------

The `registration.php` page displays the registration form. When the form is submitted, the data is sent to `process.php`, which checks the required fields.

If required information is missing, the application displays validation errors. If the submission is valid, the registration is written to `registrations.csv`.

The `result.php` page reads the saved CSV data and displays the registration records in an HTML table.

![Student Registration System results](images/Student_Registration_Results.png)

**Fig. 1. Student Registration System displaying saved registration records from the CSV file.**

[Back to Portfolio](./)
