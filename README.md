# Responsive University Website

This project is a responsive website for a university. It includes several pages such as Home, About, Courses, Blog, and Contact Us. The design is clean and modern, and the website is fully responsive, ensuring it looks good on all devices.

## Pages

- **Home:** The landing page with an introduction to the university and its offerings.
- **About:** Information about the university's history, mission, and vision.
- **Courses:** Details of the courses and programs offered.
- **Blog:** Latest news and articles related to the university.
- **Contact:** Contact information and a form for visitors to get in touch.

## Technologies Used

- HTML
- CSS
- JavaScript
- PHP
- Google Fonts
- Font Awesome

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/university-website.git
2. Setup:
- Ensure you have a local server environment (e.g., XAMPP, WAMP) for PHP files.
- Place the project files in the server's root directory.
3. Open the Website::
- Open index.html in your web browser to view the website.

## PHP Form Handler
The project includes a PHP file (form-handler.php) to handle form submissions from the Contact Us page. The PHP script processes the form data and sends an email with the submission details.

form-handler.php
<?php
$name = $_POST['name'];
$visitor_email = $_POST['email'];
$subject = $_POST['subject'];
$message = $_POST['message'];

$email_from = 'info@yourwebsite.com';
$email_subject = 'New Form Submission';
$email_body = "User Name: $name .\n".
              "User EMAIL: $visitor_email .\n". 
              "Subject: $subject .\n".
              "User Message: $message .\n";

$to = 'any_available_email@email.com';
$headers = "From: $email_from \r\n";
$headers .= "Reply-to: $visitor_email \r\n";

mail($to, $email_subject, $email_body, $headers);

header("Location: contact.html");
?>

## CSS Styles
The CSS file (styles.css) defines the styling for various components of the website. Here's a snippet of the CSS used:

* {
  margin: 0;
  padding: 0;
}

.poppins-thin {
  font-family: "Poppins", sans-serif;
  font-weight: 100;
  font-style: normal;
}

/* ... (and so on for other font weights and styles) */

.header {
  min-height: 100vh;
  width: 100%;
  background-image: linear-gradient(rgba(4, 9, 30, 0.7), rgba(4, 9, 30, 0.07)),
    url(images/banner.png);
  background-position: center;
  background-size: cover;
  position: relative;
}

/* ... (continued styles for other sections like nav, course, campus, etc.) */

## About the Project
This project showcases a responsive website design suitable for a university. It includes essential sections such as Home, About, Courses, Blog, and Contact Us. The design is implemented using HTML, CSS, and JavaScript, with additional styling and icons from Google Fonts and Font Awesome. The website is designed to be fully responsive, providing an optimal viewing experience across a wide range of devices. The PHP script handles form submissions for the Contact Us page.

## Author
This project was created by Behnam Vosoogh.


This consolidated `README.md` file includes everything about your project in one place, making it easier for users and contributors to understand, use, and set up the project locally. Adjust the URLs, paths, and content as per your actual project structure and details.






   
