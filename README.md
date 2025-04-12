<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        /* Styling for the navbar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #B22222; /* Firebrick red background */
            padding: 1rem;
        }
        nav a {
            color: #FFF5EE; /* Seashell text */
            text-decoration: none;
            margin: 0 1rem;
            font-weight: bold;
        }
        nav a:hover {
            color: #FFD700; /* Gold on hover */
            text-decoration: underline;
        }
        .navbar-links {
            display: flex;
        }
        /* Responsive design for smaller screens */
        @media (max-width: 600px) {
            .navbar-links {
                flex-direction: column;
                align-items: center;
            }
        }
        /* Styling for the contact form */
        form {
            max-width: 500px;
            margin: 2rem auto;
            padding: 1.5rem;
            border: 2px solid #B22222; /* Firebrick red border */
            border-radius: 10px;
            background-color: #FFE4E1; /* Misty rose background */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Subtle shadow */
        }
        form label {
            display: block;
            margin-bottom: 0.5rem;
            color: #B22222; /* Firebrick red text */
            font-weight: bold;
        }
        form input, form textarea, form select {
            width: 100%;
            padding: 0.5rem;
            margin-bottom: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #FFF8DC; /* Cornsilk background */
        }
        form input:focus, form textarea:focus, form select:focus {
            border-color: #B22222; /* Firebrick red border on focus */
            outline: none;
        }
        form button {
            padding: 0.7rem 1.5rem;
            background-color: #B22222; /* Firebrick red button */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
        }
        form button:hover {
            background-color: #8B0000; /* Dark red on hover */
        }
        /* Footer styling */
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #333;
            color: white;
        }
        footer p {
            margin: 0;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <h1 style="color: white;">Professional Contact</h1>
            <div class="navbar-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>
    <main>
        <p style="text-align: center; color: #B22222; font-size: 1.2rem;">We'd love to hear from you. Please fill out the form below.</p>
        <section id="contact">
            <h2 style="text-align: center; color: #B22222;">Contact Us</h2>
            <form action="#" method="post">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
                
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>
                
                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" placeholder="Enter your phone number" required>
                
                <label for="subject">Subject:</label>
                <select id="subject" name="subject" required>
                    <option value="" disabled selected>Select a subject</option>
                    <option value="general">General Inquiry</option>
                    <option value="support">Support</option>
                    <option value="feedback">Feedback</option>
                </select>
                
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" placeholder="Write your message here" required></textarea>
                
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 Your Company Name. All rights reserved.</p>
    </footer>
</body>
</html>
