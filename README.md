<h1>THE MISKATONIC TEACHING HOSPITAL STROKE PREVENTION AND REHABILITATION CENTRE WEB APPLICATION</h1>

<h2>This application is for submission as part of the Leeds Trinity University Module COM7033</h2>

This web application allows users to register, log in, upload files (CSV format), and perform basic operations securely. The app uses Flask for the backend, HTML/CSS/JavaScript for the frontend, and Google reCAPTCHA for bot protection.

<h3>Features</h3>
<li>User Registration: Secure sign-up with email verification and password hashing.</li>
<li>Login: Authentication system.</li>
<li>File Manipulation: Users can edit and delete users.</li>
<li>File Upload: Users can upload CSV files with data that is processed on the backend.</li>
<li>File Manipulation: Users can edit, add and delete data in the Stoke Dataset.</li>
<li>Bot Protection: reCAPTCHA is implemented on registration.</li>
<li>Security: The application is designed with best practices, such as input validation, and hashed passwords.</li>

<h3>Table of Contents</h3>
<ul>
<li>Installation</li>
<li>Technologies</li>
<li>App Architecture</li>
<li>Configuration</li>
<li>Usage</li>
<li>Security</li>
<li>Contributing</li>
<li>License</li>
</ul>

<h1>Web App Installation Guide</h1>

<h2>Installation</h2>

<h3>Prerequisites</h3>
<ul>
<li>Python 3.x or higher</li>
<li>Pip (for package management)</li>
</ul>
        
<h3>Steps</h3>
<ol>
<li>Clone the repository</li>            
<li>Create and activate a virtual environment</li>           
<li>Install the required dependencies</li>
<li>Set up the environment variables for the application</li>
<li>Initialize the database (if using SQLite)</li>
<li>Run the Flask app</li>
</ol>
    </section>

<h2>Technologies</h2>
        <ul>
            <li>Backend: Flask (Python)</li>
            <li>Frontend: HTML, CSS, JavaScript</li>
            <li>Database: SQLite and MongoDB</li>
            <li>reCAPTCHA: Google reCAPTCHA for bot protection</li>
            <li>File Storage: Can use local file storage or cloud services like AWS S3</li>
        </ul>

  <h2>App Architecture</h2>
        <ul>
            <li><strong>Frontend (UI)</strong>: The user interacts with a web interface that makes API calls to the Flask backend.</li>
            <li><strong>Backend</strong>: Flask app processes the business logic, including user authentication, file uploads, and integration with third-party services (reCAPTCHA).</li>
            <li><strong>Database</strong>: Stores user credentials and metadata about uploaded files.</li>
            <li><strong>Security</strong>: Bot protection via reCAPTCHA, and password hashing using Werkzeu.</li>
        </ul>


  <h2>Configuration</h2>
        <p>To configure the application:</p>
        <ul>
            <li>Set the necessary environment variables .</li>
            <li>If using a different database than SQLite (e.g., PostgreSQL), modify the database URI in <code>config.py</code>.</li>
            <li>Set up Google reCAPTCHA by creating a reCAPTCHA project in the Google reCAPTCHA Admin Console and adding the secret key to your <code>.env</code> file.</li>
        </ul>



  <h2>Usage</h2>
        <ul>
            <li><strong>User Registration</strong>: Navigate to the registration page, enter user details, and solve the reCAPTCHA challenge to sign up.</li>
            <li><strong>Login</strong>: Users can log in using their credentials, and reCAPTCHA will verify it's a human user.</li>
            <li><strong>File Upload</strong>: After logging in, users can upload CSV files. The backend processes the files and stores the information.</li>
            <li><strong>File Processing</strong>: Uploaded files are processed and stored in the database and can be viewed, edited, added and deleted.</li>
        </ul>
    </section>


  <h2>Security</h2>
        <ul>
            <li><strong>Password Hashing</strong>: All passwords are hashed using Werkzeug before storing in the database.</li>
            <li><strong>reCAPTCHA</strong>: Ensures that users are human and not bots during the registration, login, and file upload processes.</li>
            <li><strong>Session Management</strong>: User sessions are managed via Flask’s session handling (or JWT tokens).</li>
            <li><strong>Input Validation</strong>: User inputs are validated and sanitized to prevent SQL injection and XSS attacks.</li>
        </ul>
    </section>

  <h2>Contributing</h2>
        <p>Contributions are welcome after Feburary 2025 (once my assignment has been assessed)! To contribute to this project, follow these steps:</p>
        <ol>
            <li>Fork the repository.</li>
            <li>Create a new branch (git checkout -b feature-name).</li>
            <li>Commit your changes (git commit -am 'Add new feature').</li>
            <li>Push to the branch (git push origin feature-name).</li>
            <li>Open a pull request describing your changes.</li>
        </ol>


  <h2>License</h2>
        <p>This project is licensed under the MIT License - see the LICENSE file for details.</p>

