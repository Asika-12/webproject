# webproject
webproject description
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bus Ticket Booking</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="booking-container">
        <h1>Bus Ticket Booking</h1>
        <form id="ticket-booking-form">
            <div class="form-group">
                <label for="from-location">From</label>
                <input type="text" id="from-location" name="from-location" placeholder="Enter departure city" required>
            </div>
            <div class="form-group">
                <label for="to-location">To</label>
                <input type="text" id="to-location" name="to-location" placeholder="Enter destination city" required>
            </div>
            <div class="form-group">
                <label for="departure-date">Departure Date</label>
                <input type="date" id="departure-date" name="departure-date" required>
            </div>
            <div class="form-group">
                <label for="number-of-passengers">Number of Passengers</label>
                <input type="number" id="number-of-passengers" name="number-of-passengers" min="1" required>
            </div>
            <div class="form-group">
                <label for="bus-type">Bus Type</label>
                <select id="bus-type" name="bus-type" required>
                    <option value="express">Express</option>
                    <option value="sleeper">Sleeper</option>
                    <option value="luxury">Luxury</option>
                </select>
            </div>
            <div class="form-group">
                <label for="seat-selection">Select Seat(s)</label>
                <select id="seat-selection" name="seat-selection" required>
                    <option value="window">Window</option>
                    <option value="aisle">Aisle</option>
                    <option value="middle">Middle</option>
                </select>
            </div>
            <button type="submit" class="book-btn">Book Ticket</button>
        </form>
        <div id="confirmation-message"></div>
    </div>

    <script src="script.js"></script>
</body>
</html>
