# my-portoflio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tourism App</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 15px 0;
        }

        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
        }

        .container {
            margin: 20px;
        }

        .section {
            background-color: white;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .section h2 {
            color: #333;
            border-bottom: 2px solid #333;
            padding-bottom: 10px;
            margin-bottom: 15px;
        }

        .section ul {
            list-style-type: none;
            padding: 0;
        }

        .section ul li {
            padding: 8px 0;
            border-bottom: 1px solid #ddd;
        }

        .section img {
            width: 100%;
            height: auto;
            margin: 15px 0;
            border-radius: 8px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

        /* Sign-up Page */
        .signup-container {
            max-width: 500px;
            margin: 50px auto;
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .signup-container h2 {
            text-align: center;
        }

        .signup-container input {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .signup-container button {
            width: 100%;
            padding: 10px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .signup-container button:hover {
            background-color: #555;
        }

        /* Booking Form Styles */
        .booking-container {
            max-width: 600px;
            margin: 20px auto;
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .booking-container h2 {
            text-align: center;
            color: #333;
        }

        .booking-container form {
            display: flex;
            flex-direction: column;
        }

        .booking-container input, .booking-container select {
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .booking-container button {
            padding: 10px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .booking-container button:hover {
            background-color: #555;
        }

        /* Hide the booking forms by default */
        #hotelBooking, #flightBooking {
            display: none;
        }
    </style>
    <script>
        // Function to toggle visibility of hotel and flight booking forms
        function showSection(sectionId) {
            document.getElementById('hotelBooking').style.display = 'none';
            document.getElementById('flightBooking').style.display = 'none';
            document.getElementById('places').style.display = 'none';
            document.getElementById('hotels').style.display = 'none';
            document.getElementById('restaurants').style.display = 'none';
            document.getElementById('signup').style.display = 'none';

            document.getElementById(sectionId).style.display = 'block';
        }
    </script>
</head>
<body>

<header>
    <h1>Tourism App</h1>
</header>

<nav>
    <a href="javascript:void(0)" onclick="showSection('places')">Tourist Places</a>
    <a href="javascript:void(0)" onclick="showSection('hotels')">Hotels</a>
    <a href="javascript:void(0)" onclick="showSection('restaurants')">Restaurants</a>
    <a href="javascript:void(0)" onclick="showSection('hotelBooking')">Book Hotel</a>
    <a href="javascript:void(0)" onclick="showSection('flightBooking')">Book Flights</a>
    <a href="javascript:void(0)" onclick="showSection('signup')">Sign Up</a>
</nav>

<div class="container">

    <!-- Tourist Places Section -->
    <div class="section" id="places">
        <h2>Tourist Places</h2>
        <ul>
            <li><strong>Eiffel Tower:</strong> Iconic Paris landmark - Price: $30</li>
            <img src="https://example.com/eiffel.jpg" alt="Eiffel Tower">
            <li><strong>Colosseum:</strong> Ancient Roman amphitheater - Price: $20</li>
            <img src="https://example.com/colosseum.jpg" alt="Colosseum">
            <li><strong>Great Wall of China:</strong> Historical structure - Price: $25</li>
            <img src="https://example.com/greatwall.jpg" alt="Great Wall of China">
            <li><strong>Taj Mahal:</strong> Mausoleum in India - Price: $15</li>
            <img src="https://example.com/tajmahal.jpg" alt="Taj Mahal">
        </ul>
    </div>

    <!-- Hotels Section -->
    <div class="section" id="hotels">
        <h2>Hotels</h2>
        <ul>
            <li><strong>Hilton Hotel:</strong> 5-star luxury hotel - Price: $200 per night</li>
            <img src="https://example.com/hilton.jpg" alt="Hilton Hotel">
            <li><strong>Marriott Hotel:</strong> Premium service hotel - Price: $180 per night</li>
            <img src="https://example.com/marriott.jpg" alt="Marriott Hotel">
            <li><strong>Holiday Inn:</strong> Affordable stay - Price: $100 per night</li>
            <img src="https://example.com/holidayinn.jpg" alt="Holiday Inn">
            <li><strong>Radisson Blu:</strong> Comfortable and stylish - Price: $150 per night</li>
            <img src="https://example.com/radisson.jpg" alt="Radisson Blu">
        </ul>
    </div>

    <!-- Restaurants Section -->
    <div class="section" id="restaurants">
        <h2>Restaurants</h2>
        <ul>
            <li><strong>Le Gourmet:</strong> Fine French cuisine - Avg. Price: $60 per person</li>
            <img src="https://example.com/legourmet.jpg" alt="Le Gourmet">
            <li><strong>La Piazza:</strong> Italian trattoria - Avg. Price: $50 per person</li>
            <img src="https://example.com/lapiazza.jpg" alt="La Piazza">
            <li><strong>Sushi Zen:</strong> Authentic Japanese sushi - Avg. Price: $40 per person</li>
            <img src="https://example.com/sushizen.jpg" alt="Sushi Zen">
            <li><strong>El Asador:</strong> Argentinian steakhouse - Avg. Price: $55 per person</li>
            <img src="https://example.com/elasador.jpg" alt="El Asador">
        </ul>
    </div>

    <!-- Hotel Booking Section -->
    <div class="booking-container" id="hotelBooking">
        <h2>Book a Hotel Room</h2>
        <form>
            <input type="text" name="fullname" placeholder="Full Name" required>
            <input type="email" name="email" placeholder="Email Address" required>
            <select name="hotel">
                <option value="Hilton">Hilton Hotel - $200 per night</option>
                <option value="Marriott">Marriott Hotel - $180 per night</option>
                <option value="Holiday Inn">Holiday Inn - $100 per night</option>
                <option value="Radisson Blu">Radisson Blu - $150 per night</option>
                <option value="Four Seasons">Four Seasons - $250 per night</option>
            </select>
            <input type="date" name="checkin" required>
            <input type="date" name="checkout" required>
            <button type="submit">Book Now</button>
        </form>
    </div>

    <!-- Flight Booking Section -->
    <div class="booking-container" id="flightBooking">
        <h2>Book a Flight</h2>
        <form>
            <input type="text" name="fullname" placeholder="Full Name" required>
            <input type="email" name="email" placeholder="Email Address" required>
            <input type="text" name="from" placeholder="Departure City" required>
            <input type="text" name="to" placeholder="Destination City" required>
            <input type="date" name="departure" required>
            <input type="date" name="return">
            <button type="submit">Book Flight</button>
        </form>
    </div>

    <!-- Sign Up Section -->
    <div class="signup-container" id="signup">
        <h2>Sign Up</h2>
        <form>
            <input type="text" name="fullname" placeholder="Full Name" required>
            <input type="email" name="email" placeholder="Email Address" required>
            <input type="password" name="password" placeholder="Password" required>
            <input type="password" name="confirmpassword" placeholder="Confirm Password" required>
            <button type="submit">Sign Up</button>
        </form>
    </div>

</div>

<footer>
    <p>&copy; 2024 Tourism App. All Rights Reserved.</p>
</footer>

</body>
</html>
