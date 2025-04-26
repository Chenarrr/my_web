<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chenar's Personal Web</title>
    <style>
        /* General dark theme styling */
        body {
            background-color: #121212; /* Dark background */
            color: #E0E0E0; /* Light text */
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #1F1F1F; /* Darker navbar background */
            padding: 1rem;
        }
        nav a {
            color: #BB86FC; /* Purple text */
            text-decoration: none;
            margin: 0 1rem;
            font-weight: bold;
        }
        nav a:hover {
            color: #03DAC6; /* Teal on hover */
            text-decoration: underline;
        }
        .navbar-links {
            display: flex;
        }
        @media (max-width: 600px) {
            .navbar-links {
                flex-direction: column;
                align-items: center;
            }
        }
        form {
            max-width: 500px;
            margin: 2rem auto;
            padding: 1.5rem;
            border: 2px solid #BB86FC; /* Purple border */
            border-radius: 10px;
            background-color: #1E1E1E; /* Dark form background */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5); /* Subtle shadow */
        }
        form label {
            display: block;
            margin-bottom: 0.5rem;
            color: #BB86FC; /* Purple text */
            font-weight: bold;
        }
        form input, form textarea, form select {
            width: 100%;
            padding: 0.5rem;
            margin-bottom: 1rem;
            border: 1px solid #03DAC6; /* Teal border */
            border-radius: 5px;
            background-color: #2C2C2C; /* Dark input background */
            color: #E0E0E0; /* Light text */
        }
        form input:focus, form textarea:focus, form select:focus {
            border-color: #BB86FC; /* Purple border on focus */
            outline: none;
        }
        form button {
            padding: 0.7rem 1.5rem;
            background-color: #BB86FC; /* Purple button */
            color: #121212; /* Dark text */
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
        }
        form button:hover {
            background-color: #3700B3; /* Darker purple on hover */
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #1F1F1F; /* Darker footer background */
            color: #E0E0E0; /* Light text */
        }
        footer p {
            margin: 0;
        }
        p {
            text-align: center;
            color: #E0E0E0; /* Light text */
            font-size: 1.2rem;
        }
        h1, h2 {
            text-align: center;
            color: #BB86FC; /* Purple text */
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <h1>Chenar's Personal Web</h1>
            <div class="navbar-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>
    <main>
        <p>Welcome to Chenar's personal webpage. Please fill out the form below to share your information with me.</p>
        <section id="contact">
            <h2>Contact Me</h2>
            <form action="#" method="post" enctype="multipart/form-data">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
                
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>
                
                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" placeholder="Enter your phone number" required>
                
                <label for="address">Address:</label>
                <input type="text" id="address" name="address" placeholder="Enter your address" required>
                
                <label for="contact-method">Preferred Contact Method:</label>
                <select id="contact-method" name="contact-method" required>
                    <option value="" disabled selected>Select a contact method</option>
                    <option value="email">Email</option>
                    <option value="phone">Phone</option>
                    <option value="text">Text Message</option>
                </select>
                
                <label for="subject">Subject:</label>
                <select id="subject" name="subject" required>
                    <option value="" disabled selected>Select a subject</option>
                    <option value="general">General Inquiry</option>
                    <option value="support">Support</option>
                    <option value="feedback">Feedback</option>
                </select>
                
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" placeholder="Write your message here" required></textarea>
                
                <label for="file">Upload a File (optional):</label>
                <input type="file" id="file" name="file">
                
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Chenar. All rights reserved.</p>
    </footer>
</body>
</html>
