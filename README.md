# Job Portal Web Application

This repository contains a Job Portal Web Application designed to connect job seekers with potential employers. The platform provides a user-friendly interface for job seekers to search and apply for job openings while allowing employers to post job listings and manage candidate applications.

## Features

- **User Authentication**: Secure login and registration for both job seekers and employers.
- **Job Search**: Advanced search functionality to filter job listings based on various criteria.
- **Job Application**: Easy application process for job seekers to apply for multiple job openings.
- **Employer Dashboard**: Tools for employers to post job listings and manage candidate applications.
- **Notifications**: Alerts and notifications for job seekers on application status and new job postings.
- **Responsive Design**: Optimized for both desktop and mobile use.

## Screenshots

(Need to add screenshots of the web application here to give users a visual understanding of the platform.)

## Installation

To get a local copy up and running, follow these simple steps.

### Prerequisites

- PHP
- MySQL
- Apache or any web server that supports PHP

### Clone the Repository

```bash
git clone https://github.com/fayazmohammad2002/JOB-PORTAL.git
```

### Set Up the Database

1. Create a MySQL database.
2. Import the provided SQL file into your database. This file is usually named `database.sql` and is located in the root directory of the repository.

```sql
CREATE DATABASE job_portal;
USE job_portal;
SOURCE /path_to_your_cloned_repo/JOB-PORTAL/database.sql;
```

### Configure the Application

1. Locate the `config.php` file in the root directory.
2. Update the database configuration details.

```php
<?php
$servername = "localhost";
$username = "your_username";
$password = "your_password";
$dbname = "job_portal";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
```

### Deploy the Application

1. Copy the cloned repository files to your web server's root directory (e.g., `htdocs` for XAMPP, `www` for WAMP).
2. Start your web server and navigate to `http://localhost/JOB-PORTAL` in your web browser.

## Usage

1. **Sign Up**: Register as either a job seeker or an employer.
2. **Login**: Use your credentials to log in.
3. **Job Seekers**:
   - Search for job openings using the search functionality.
   - Apply for jobs directly through the platform.
   - Track the status of your applications.
4. **Employers**:
   - Post new job listings.
   - Manage applications from candidates.
   - Communicate with potential hires.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Fayaz Mohammad - [LinkedIn](https://www.linkedin.com/in/fayazmohammad2002) - [Email](mailto:fayazmohammad2002@gmail.com)

Project Link: [https://github.com/fayazmohammad2002/JOB-PORTAL](https://github.com/fayazmohammad2002/JOB-PORTAL)

---

*The Job Portal Web Application is designed to bridge the gap between job seekers and employers, providing a seamless and efficient platform for job search and recruitment.*
