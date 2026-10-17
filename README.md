<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Islamic Wedding Invitation - A & M</title>
    <!-- Google Fonts: Elegant and complementary -->
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Marcellus&family=Tajawal:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        /* Color Palette & Islamic Elements */
        :root {
            --bg-color: #f6faf2;          /* Very light green background */
            --primary-green: #1a4d2e;     /* Rich Islamic Green */
            --accent-green: #0a2d1a;       /* Dark Green */
            --primary-gold: #c6a059;      /* Metallic/Matte Gold */
            --dark-gold: #9c7b41;         /* Darker shading gold */
            --text-on-dark: #fffdf9;
            --text-on-light: #2c2c2c;
            --font-main: 'Tajawal', sans-serif;
            --font-header: 'Marcellus', serif;
            --font-cursive: 'Great Vibes', cursive;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: var(--font-main);
            background-color: var(--bg-color);
            color: var(--text-on-light);
            line-height: 1.8;
            text-align: center;
            overflow-x: hidden;
        }

        /* --- Header / Hero Section --- */
        header {
            position: relative;
            /* Islamic pattern background over a dark green gradient */
            background: linear-gradient(rgba(10, 45, 26, 0.85), rgba(26, 77, 46, 0.85)), 
                        url('https://images.unsplash.com/photo-1606103901170-eb3c87e59c6c?q=80&w=2000') no-repeat center center/cover;
            color: var(--text-on-dark);
            padding: 120px 20px 80px;
            min-height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-bottom: 8px solid var(--primary-gold);
        }

        /* Gold border elements (simple illustration) */
        header::before, header::after {
            content: "";
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--primary-gold);
            height: 2px;
            width: 80px;
        }

        header::before { top: 60px; }
        header::after { bottom: 60px; }

        .bismillah {
            font-size: 1.6rem;
            margin-bottom: 15px;
            color: var(--primary-gold);
            font-weight: 500;
        }

        .basmala-text {
            font-family: 'Times New Roman', Times, serif; /* Basic Arabic fallback */
            font-size: 2.2rem;
            margin-bottom: 10px;
        }

        .couple-names {
            font-family: var(--font-cursive);
            font-size: 5rem;
            margin-bottom: 25px;
            color: var(--primary-gold);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .invitation-date {
            font-size: 1.4rem;
            letter-spacing: 3px;
            text-transform: uppercase;
            color: #d8c3a5; /* Softer Gold */
        }

        /* --- Sections --- */
        section {
            padding: 80px 20px;
            max-width: 900px;
            margin: 0 auto;
        }

        .section-title {
            font-family: var(--font-cursive);
            font-size: 3.5rem;
            color: var(--primary-green);
            margin-bottom: 25px;
        }

        h2 {
            font-family: var(--font-header);
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 20px;
            color: var(--primary-green);
        }

        .islamic-greeting {
            font-size: 1.3rem;
            color: var(--primary-gold);
            margin-bottom: 10px;
            font-weight: 500;
        }

        p {
            font-size: 1.1rem;
            margin-bottom: 30px;
            color: var(--text-on-light);
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        /* --- Details Cards --- */
        .details-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }

        .card {
            background-color: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            border-top: 5px solid var(--primary-gold);
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            font-family: var(--font-header);
            font-size: 1.6rem;
            margin-bottom: 20px;
            color: var(--primary-gold);
            text-transform: uppercase;
        }

        .detail-item {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin-bottom: 15px;
            font-size: 1.1rem;
        }

        .icon {
            font-size: 1.3rem;
            color: var(--primary-green);
        }

        .btn {
            display: inline-block;
            margin-top: 25px;
            padding: 12px 35px;
            background-color: var(--primary-green);
            color: var(--text-on-dark);
            text-decoration: none;
            border-radius: 30px;
            font-weight: 500;
            font-size: 1rem;
            transition: all 0.3s ease;
            border: 2px solid var(--primary-green);
        }

        .btn:hover {
            background-color: var(--bg-color);
            color: var(--primary-green);
            border: 2px solid var(--primary-gold);
        }

        /* --- RSVP Section --- */
        form {
            background-color: #fff;
            padding: 50px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            max-width: 600px;
            margin: 0 auto;
            text-align: left;
            border: 2px solid var(--primary-gold);
        }

        form label {
            display: block;
            margin-bottom: 10px;
            font-weight: 500;
            color: var(--accent-green);
        }

        form input, form select, form textarea {
            width: 100%;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 8px;
            margin-bottom: 25px;
            font-family: var(--font-main);
            background-color: #fafdf8;
        }

        button.btn {
            border: none;
            cursor: pointer;
            width: 100%;
            font-size: 1.1rem;
        }

        /* --- Music Control Button (Floating) --- */
        #music-control {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
            width: 50px;
            height: 50px;
            background-color: var(--primary-gold);
            color: var(--text-on-dark);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.5rem;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            border: none;
            cursor: pointer;
            opacity: 0.9;
            transition: all 0.3s ease;
        }

        #music-control:hover {
            opacity: 1;
            transform: scale(1.1);
        }

        /* FontAwesome for music icons (added dynamically) */
        @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css');

        /* --- Footer --- */
        footer {
            background-color: #121212;
            color: #ccc;
            padding: 40px 20px;
            font-size: 1rem;
            margin-top: 60px;
        }

        footer p { color: #aaa; margin-bottom: 10px; font-size: 0.95rem; }

        @media (max-width: 768px) {
            .couple-names { font-size: 3.5rem; }
            .section-title { font-size: 2.8rem; }
            header { padding-top: 100px; }
            form { padding: 30px; }
        }
    </style>
</head>
<body>

    <!-- Background Audio Element -->
    <!-- You will need to find the specific direct link for the MP3 and replace the source URL below. 
         Free MP3 sources for this specific song are hard to find reliably, 
         you can explore platforms like archive.org or other reliable sources.
         Alternatively, you can ask a friend to host the file on a server or place it 
         directly into your GitHub repo folder if you find a suitable version.
         Assuming we will put the audio file in the same folder as index.html called 'music.mp3'
    -->
    <audio id="backgroundAudio" loop>
        <source src="music.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <!-- Music Control Button -->
    <button id="music-control" onclick="toggleMusic()">
        <i id="music-icon" class="fas fa-play"></i>
    </button>

    <!-- Header Section -->
    <header>
        <div class="islamic-greeting">As-Salamu Alaykum Wa Rahmatullahi Wa Barakatuh</div>
        <div class="bismillah">In the Name of Allah, Most Gracious, Most Merciful</div>
        <div class="basmala-text">﷽</div>
        <h1 class="couple-names">Adam & Miriam</h1>
        <p class="invitation-date">Saturday, August 15, 2026</p>
    </header>

    <!-- Welcome Section -->
    <section>
        <h2 class="section-title">The Invitation</h2>
        <p>It is with great joy and humble hearts, in gratitude to Allah (SWT), that we invite you to celebrate our union.</p>
        
        <blockquote style="font-style: italic; color: #555; border-left: 3px solid #ddd; padding-left: 15px; margin-bottom: 25px; text-align: center;">
            <p style="font-size: 1rem; color: #555;">"And among His signs is that He created for you mates from among yourselves, that you may find tranquility in them; and He placed between you affection and mercy." (Surah Ar-Rum 30:21)</p>
        </blockquote>
    </section>

    <!-- Event Details Cards -->
    <section>
        <h2 class="section-title">The Celebrations</h2>
        <div class="details-grid">
            
            <!-- Nikkah/Ceremony Card -->
            <div class="card">
                <h3>The Nikkah Ceremony</h3>
                <div class="detail-item">
                    <span class="icon"><i class="fas fa-clock"></i></span>
                    <p><strong>Time:</strong> 11:00 AM SHARP</p>
                </div>
                <div class="detail-item">
                    <span class="icon"><i class="fas fa-mosque"></i></span>
                    <p><strong>Venue:</strong> Masjid Al-Nur Central Hall</p>
                </div>
                <p>123 Faith Lane, City, State</p>
                <p>We kindly request you to arrive before the commencement of the Nikkah Khutbah.</p>
                <a href="https://maps.google.com" target="_blank" class="btn">View on Map</a>
            </div>
            
            <!-- Walima/Reception Card -->
            <div class="card">
                <h3>The Walima Dinner</h3>
                <div class="detail-item">
                    <span class="icon"><i class="fas fa-utensils"></i></span>
                    <p><strong>Time:</strong> 7:00 PM</p>
                </div>
                <div class="detail-item">
                    <span class="icon"><i class="fas fa-calendar-day"></i></span>
                    <p><strong>Date:</strong> Sunday, August 16, 2026</p>
                </div>
                <div class="detail-item">
                    <span class="icon"><i class="fas fa-building"></i></span>
                    <p><strong>Venue:</strong> The Grand Banquet Hall</p>
                </div>
                <p>456 Celebration Boulevard, City, State</p>
                <a href="https://maps.google.com" target="_blank" class="btn">View on Map</a>
            </div>
        </div>
    </section>

    <!-- RSVP Section -->
    <section>
        <h2 class="section-title">RSVP</h2>
        <p>Please share your presence with us. We kindly request responses before July 1st, 2026.</p>
        <form id="rsvpForm" onsubmit="handleRSVP(event)">
            <div>
                <label for="name">Full Name</label>
                <input type="text" id="name" required placeholder="Enter your full name">
            </div>
            
            <div>
                <label for="attendance">Will you attend?</label>
                <select id="attendance" required>
                    <option value="">Please select</option>
                    <option value="yes">Will Attend (Bi'idhnillaah)</option>
                    <option value="no">Unable to Attend</option>
                </select>
            </div>
            
            <div>
                <label for="wishes">Wishes for the Couple (Optional)</label>
                <textarea id="wishes" rows="4" placeholder="May Allah bless you..."></textarea>
            </div>
            <button type="submit" class="btn">Send My RSVP</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>Made with love. Baraka Allahu Lakuma.</p>
        <p>&copy; 2026 A & M Wedding. All Rights Reserved.</p>
    </footer>

    <!-- JavaScript for RSVP and Music Control -->
    <script>
        // --- Music Control ---
        const audio = document.getElementById("backgroundAudio");
        const musicBtn = document.getElementById("music-control");
        const musicIcon = document.getElementById("music-icon");
        let isPlaying = false;

        function toggleMusic() {
            if (isPlaying) {
                audio.pause();
                musicIcon.classList.remove("fa-pause");
                musicIcon.classList.add("fa-play");
                musicBtn.style.opacity = 0.9;
            } else {
                audio.play();
                musicIcon.classList.remove("fa-play");
                musicIcon.classList.add("fa-pause");
                musicBtn.style.opacity = 1;
            }
            isPlaying = !isPlaying;
        }

        // --- RSVP Handler ---
        function handleRSVP(event) {
            event.preventDefault(); // Prevents the form from submitting normally
            const name = document.getElementById("name").value;
            alert(`JazakAllah Khair, ${name}! Your RSVP has been received.`);
            document.getElementById("rsvpForm").reset(); // Resets the form
        }
    </script>

</body>
</html>
