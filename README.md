<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Wedding Celebration</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #8c6d46;
            --accent-color: #f7f3ed;
            --text-color: #333333;
            --light-bg: #faf7f2;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--light-bg);
            color: var(--text-color);
            line-height: 1.6;
            text-align: center;
        }

        header {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            color: white;
            padding: 100px 20px;
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        .save-the-date {
            font-size: 1.2rem;
            letter-spacing: 3px;
            text-transform: uppercase;
            margin-bottom: 15px;
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 4.5rem;
            margin-bottom: 20px;
            color: #fceade;
        }

        .wedding-date {
            font-size: 1.4rem;
            font-weight: 300;
            letter-spacing: 2px;
        }

        section {
            padding: 60px 20px;
            max-width: 800px;
            margin: 0 auto;
        }

        .section-title {
            font-family: 'Great Vibes', cursive;
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 20px;
        }

        p {
            font-size: 1.05rem;
            margin-bottom: 30px;
            color: #555;
        }

        /* Countdown Timer */
        .countdown-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
        }

        .countdown-box {
            background: white;
            padding: 15px 20px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            min-width: 80px;
        }

        .countdown-number {
            font-size: 1.8rem;
            font-weight: 600;
            color: var(--primary-color);
        }

        .countdown-label {
            font-size: 0.8rem;
            text-transform: uppercase;
            color: #777;
            margin-top: 5px;
        }

        /* Details Cards */
        .details-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
        }

        .card h3 {
            font-size: 1.4rem;
            margin-bottom: 15px;
            color: var(--primary-color);
        }

        .btn {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 25px;
            background-color: var(--primary-color);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-size: 0.9rem;
            transition: background 0.3s ease;
        }

        .btn:hover {
            background-color: #725534;
        }

        /* RSVP Form */
        form {
            background: white;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
            display: flex;
            flex-direction: column;
            gap: 20px;
            text-align: left;
        }

        label {
            font-weight: 500;
            font-size: 0.9rem;
        }

        input, select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-family: inherit;
            margin-top: 5px;
        }

        button.btn {
            border: none;
            cursor: pointer;
            width: 100%;
            font-size: 1rem;
            padding: 12px;
        }

        footer {
            background-color: #2c2c2c;
            color: #aaa;
            padding: 30px 20px;
            font-size: 0.9rem;
        }

        @media (max-width: 600px) {
            h1 { font-size: 3.5rem; }
            header { padding: 60px 15px; }
        }
    </style>
</head>
<body>

    <!-- Header / Hero Section -->
    <header>
        <div class="save-the-date">Save The Date</div>
        <h1>Eclipse & Groom</h1>
        <p class="wedding-date">December 19, 2026</p>
    </header>

    <!-- Our Story / Welcome -->
    <section>
        <h2 class="section-title">We Are Getting Married!</h2>
        <p>Together with our families, we invite you to share in our joy as we exchange our vows and begin our new chapter together. Your presence would make our special day complete.</p>
        
        <!-- Countdown Timer -->
        <div class="countdown-container">
            <div class="countdown-box">
                <div class="countdown-number" id="days">00</div>
                <div class="countdown-label">Days</div>
            </div>
            <div class="countdown-box">
                <div class="countdown-number" id="hours">00</div>
                <div class="countdown-label">Hours</div>
            </div>
            <div class="countdown-box">
                <div class="countdown-number" id="minutes">00</div>
                <div class="countdown-label">Mins</div>
            </div>
            <div class="countdown-box">
                <div class="countdown-number" id="seconds">00</div>
                <div class="countdown-label">Secs</div>
            </div>
        </div>
    </section>

    <!-- Event Details -->
    <section>
        <h2 class="section-title">The Events</h2>
        <div class="details-grid">
            <div class="card">
                <h3>The Ceremony</h3>
                <p><strong>Time:</strong> 10:00 AM</p>
                <p><strong>Venue:</strong> Grace Cathedral Hall</p>
                <p>123 Celebration Avenue, City</p>
                <a href="https://maps.google.com" target="_blank" class="btn">View on Map</a>
            </div>
            <div class="card">
                <h3>The Reception</h3>
                <p><strong>Time:</strong> 2:00 PM</p>
                <p><strong>Venue:</strong> The Royal Event Centre</p>
                <p>456 Harmony Boulevard, City</p>
                <a href="https://maps.google.com" target="_blank" class="btn">View on Map</a>
            </div>
        </div>
    </section>

    <!-- RSVP Section -->
    <section>
        <h2 class="section-title">RSVP</h2>
        <p>Please let us know if you will be able to celebrate with us by December 1st.</p>
        <form id="rsvpForm" onsubmit="handleRSVP(event)">
            <div>
                <label for="name">Full Name</label>
                <input type="text" id="name" required placeholder="Enter your full name">
            </div>
            <div>
                <label for="attendance">Will you attend?</label>
                <select id="attendance" required>
                    <option value="">Please select</option>
                    <option value="yes">Joyfully Accepts</option>
                    <option value="no">Regretfully Declines</option>
                </select>
            </div>
            <div>
                <label for="message">Wishes for the Couple (Optional)</label>
                <textarea id="message" rows="3" placeholder="Leave a sweet note..."></textarea>
            </div>
            <button type="submit" class="btn">Send RSVP</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Eclipse & Groom. Made with love.</p>
    </footer>

    <!-- JavaScript for Countdown and RSVP -->
    <script>
        // Countdown Timer Logic (Target Date: Dec 19, 2026)
        const weddingDate = new Date("December 19, 2026 10:00:00").getTime();

        function updateCountdown() {
            const now = new Date().getTime();
            const distance = weddingDate - now;

            if (distance < 0) {
                document.querySelector(".countdown-container").innerHTML = "<h3>The Wedding Day is Here!</h3>";
                return;
            }

            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

            document.getElementById("days").innerText = String(days).padStart(2, '0');
            document.getElementById("hours").innerText = String(hours).padStart(2, '0');
            document.getElementById("minutes").innerText = String(minutes).padStart(2, '0');
            document.getElementById("seconds").innerText = String(seconds).padStart(2, '0');
        }

        setInterval(updateCountdown, 1000);
        updateCountdown();

        // RSVP Handler (Simple alert mockup)
        function handleRSVP(event) {
            event.preventDefault();
            const name = document.getElementById("name").value;
            alert(`Thank you, ${name}! Your RSVP has been received.`);
            document.getElementById("rsvpForm").reset();
        }
    </script>
</body>
</html>
