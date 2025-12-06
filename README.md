# alexshilpa_wedding_2025
Wedding Invitation Card

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex & Shilpa - Holy Matrimony</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Crimson+Text:wght@400;600;700&family=Marcellus&family=Playfair+Display:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --gold: #D4AF37;
            --maroon: #800000;
            --ivory: #FFFFF0;
            --dark-red: #8B0000;
            --light-gold: #F5E8AA;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Crimson Text', serif;
            background-color: var(--ivory);
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        /* Kerala-inspired decorative elements */
        .kerala-border {
            position: relative;
            padding: 20px;
        }
        
        .kerala-border::before {
            content: "";
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80%;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--gold), transparent);
        }
        
        .kerala-border::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80%;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--gold), transparent);
        }
        
        /* Floating flowers */
        .flower {
            position: absolute;
            opacity: 0.3;
            z-index: 0;
        }
        
        .flower-1 {
            top: 10%;
            left: 5%;
            font-size: 2rem;
            color: var(--gold);
            transform: rotate(15deg);
        }
        
        .flower-2 {
            top: 15%;
            right: 5%;
            font-size: 2.5rem;
            color: var(--maroon);
            transform: rotate(-10deg);
        }
        
        .flower-3 {
            bottom: 20%;
            left: 10%;
            font-size: 2rem;
            color: var(--gold);
            transform: rotate(30deg);
        }
        
        .flower-4 {
            bottom: 10%;
            right: 10%;
            font-size: 2.5rem;
            color: var(--maroon);
            transform: rotate(-20deg);
        }
        
        /* Header */
        .header {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                        url('https://images.unsplash.com/photo-1519741497674-611481863552?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80');
            background-size: cover;
            background-position: center;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 20px;
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: "💒";
            position: absolute;
            top: 20px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 3rem;
            opacity: 0.1;
        }
        
        .header-title {
            font-family: 'Marcellus', serif;
            font-size: 4rem;
            margin-bottom: 1rem;
            color: var(--light-gold);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            letter-spacing: 2px;
        }
        
        .header-subtitle {
            font-size: 1.8rem;
            margin-bottom: 2rem;
            color: var(--light-gold);
            font-weight: 300;
            max-width: 800px;
        }
        
        .scripture {
            font-size: 1.3rem;
            font-style: italic;
            margin: 2rem 0;
            padding: 1.5rem;
            border-left: 3px solid var(--gold);
            background-color: rgba(0, 0, 0, 0.5);
            max-width: 800px;
            border-radius: 5px;
        }
        
        /* Couple Section */
        .couple-section {
            padding: 5rem 2rem;
            position: relative;
            background-color: #fff;
        }
        
        .couple-container {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 4rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .groom, .bride {
            text-align: center;
            flex: 1;
            min-width: 300px;
        }
        
        .couple-photo {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            border: 8px solid var(--gold);
            object-fit: cover;
            margin-bottom: 1.5rem;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        
        .couple-name {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: var(--dark-red);
            margin-bottom: 0.5rem;
        }
        
        .couple-desc {
            font-size: 1.2rem;
            color: #555;
            margin-bottom: 0.5rem;
        }
        
        .couple-parents {
            font-size: 1.1rem;
            color: #777;
            font-style: italic;
            margin-top: 1rem;
        }
        
        .and {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            color: var(--gold);
            font-weight: bold;
            position: relative;
        }
        
        /* Details Section */
        .details-section {
            padding: 5rem 2rem;
            background-color: #f9f5f0;
            position: relative;
        }
        
        .details-container {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
        }
        
        .section-title {
            font-family: 'Marcellus', serif;
            font-size: 3rem;
            color: var(--dark-red);
            margin-bottom: 3rem;
            position: relative;
            display: inline-block;
        }
        
        .section-title::after {
            content: "";
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background-color: var(--gold);
        }
        
        .date-time {
            font-size: 2.5rem;
            color: var(--maroon);
            margin-bottom: 1.5rem;
            font-weight: bold;
        }
        
        .date-subtext {
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 2rem;
        }
        
        .venue-card {
            background-color: white;
            border-radius: 10px;
            padding: 2.5rem;
            margin: 2rem auto;
            max-width: 800px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            border-top: 5px solid var(--gold);
        }
        
        .venue-name {
            font-size: 2rem;
            color: var(--dark-red);
            margin-bottom: 1rem;
        }
        
        .venue-address {
            font-size: 1.2rem;
            color: #555;
            margin-bottom: 1.5rem;
        }
        
        .reception-card {
            background-color: white;
            border-radius: 10px;
            padding: 2rem;
            margin: 2rem auto;
            max-width: 800px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            border-left: 5px solid var(--maroon);
        }
        
        /* Map Section */
        .map-section {
            padding: 3rem 2rem;
            background-color: white;
        }
        
        .map-container {
            max-width: 1000px;
            margin: 0 auto;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Prayer Section */
        .prayer-section {
            padding: 5rem 2rem;
            background-color: #f0e8dd;
            text-align: center;
        }
        
        .prayer-text {
            font-size: 1.5rem;
            color: #555;
            max-width: 800px;
            margin: 0 auto 3rem;
            font-style: italic;
        }
        
        /* Countdown */
        .countdown {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 3rem 0;
            flex-wrap: wrap;
        }
        
        .countdown-item {
            background-color: white;
            border-radius: 10px;
            padding: 1.5rem;
            min-width: 120px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            border: 1px solid var(--light-gold);
        }
        
        .countdown-number {
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--dark-red);
            display: block;
        }
        
        .countdown-label {
            font-size: 1rem;
            color: #777;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        /* Footer */
        .footer {
            padding: 3rem 2rem;
            background-color: var(--dark-red);
            color: white;
            text-align: center;
        }
        
        .footer-text {
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }
        
        .footer-verse {
            font-size: 1.3rem;
            font-style: italic;
            margin: 2rem 0;
            color: var(--light-gold);
        }
        
        .footer-note {
            font-size: 1.1rem;
            margin-top: 2rem;
            color: #ddd;
        }
        
        /* Button */
        .prayer-btn {
            background-color: var(--gold);
            color: var(--dark-red);
            border: none;
            padding: 1rem 2.5rem;
            font-size: 1.2rem;
            border-radius: 50px;
            cursor: pointer;
            font-family: 'Crimson Text', serif;
            font-weight: bold;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(212, 175, 55, 0.3);
        }
        
        .prayer-btn:hover {
            background-color: var(--dark-red);
            color: white;
            transform: translateY(-3px);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-title {
                font-size: 2.5rem;
            }
            
            .header-subtitle {
                font-size: 1.3rem;
            }
            
            .couple-name {
                font-size: 2rem;
            }
            
            .date-time {
                font-size: 1.8rem;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
            
            .and {
                font-size: 3rem;
            }
            
            .flower {
                display: none;
            }
        }
        
        /* Animation */
        @keyframes float {
            0%, 100% {
                transform: translateY(0) rotate(0deg);
            }
            50% {
                transform: translateY(-20px) rotate(5deg);
            }
        }
        
        .flower {
            animation: float 6s ease-in-out infinite;
        }
        
        .flower-2 {
            animation-delay: 1s;
        }
        
        .flower-3 {
            animation-delay: 2s;
        }
        
        .flower-4 {
            animation-delay: 3s;
        }
        
        /* Save the date */
        .save-date {
            background-color: var(--maroon);
            color: white;
            padding: 0.7rem 1.5rem;
            border-radius: 50px;
            font-size: 1.1rem;
            margin-top: 2rem;
            display: inline-block;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .save-date:hover {
            background-color: var(--dark-red);
            transform: scale(1.05);
        }
        
        /* Heart animation */
        .heart {
            color: var(--maroon);
            display: inline-block;
            animation: heartbeat 1.5s ease-in-out infinite;
        }
        
        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }
    </style>
</head>
<body>
    <!-- Decorative Flowers -->
    <div class="flower flower-1">🌸</div>
    <div class="flower flower-2">💮</div>
    <div class="flower flower-3">🏵️</div>
    <div class="flower flower-4">🌺</div>
    
    <!-- Header Section -->
    <header class="header">
        <div class="kerala-border">
            <h1 class="header-title">Alex & Shilpa</h1>
            <p class="header-subtitle">cordially invite you to their Holy Matrimony</p>
            
            <div class="scripture">
                <p>"I have found the one whom my soul loves."</p>
                <p>- Song of Solomon 3:4</p>
            </div>
            
            <div class="scripture">
                <p>"Therefore what God has joined together, let no one separate."</p>
                <p>- Mark 10:9</p>
            </div>
            
            <div class="countdown">
                <div class="countdown-item">
                    <span class="countdown-number" id="days">00</span>
                    <span class="countdown-label">Days</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-number" id="hours">00</span>
                    <span class="countdown-label">Hours</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-number" id="minutes">00</span>
                    <span class="countdown-label">Minutes</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-number" id="seconds">00</span>
                    <span class="countdown-label">Seconds</span>
                </div>
            </div>
            
            <a href="#details" class="save-date">
                <i class="fas fa-calendar-alt"></i> Save the Date
            </a>
        </div>
    </header>
    
    <!-- Couple Section -->
    <section class="couple-section">
        <div class="couple-container">
            <div class="groom">
                <div class="couple-photo-placeholder">
                    <!-- Replace with actual photo -->
                    <div class="couple-photo" style="background: linear-gradient(135deg, #f5e8aa, #d4af37); display: flex; align-items: center; justify-content: center; color: var(--dark-red); font-size: 3rem;">
                        AY
                    </div>
                </div>
                <h2 class="couple-name">Alex Yohannan</h2>
                <p class="couple-desc">Son of</p>
                <p class="couple-parents">Mr. T Yohannan & Mrs. Susan Yohannan</p>
                <p class="couple-desc">Konnayil Saji Bhavan, Vallikunnam</p>
                <p class="couple-desc">Alappuzha, Kerala</p>
            </div>
            
            <div class="and">
                <span class="heart">❤️</span>
                <div style="font-size: 1.5rem; color: var(--maroon); margin-top: 1rem;">&</div>
            </div>
            
            <div class="bride">
                <div class="couple-photo-placeholder">
                    <!-- Replace with actual photo -->
                    <div class="couple-photo" style="background: linear-gradient(135deg, #f5e8aa, #d4af37); display: flex; align-items: center; justify-content: center; color: var(--dark-red); font-size: 3rem;">
                        SS
                    </div>
                </div>
                <h2 class="couple-name">Shilpa Shyam</h2>
                <p class="couple-desc">Daughter of</p>
                <p class="couple-parents">Mr. K.C. Shyam & Mrs. Sunija Shyam</p>
                <p class="couple-desc">Rehoboth House</p>
                <p class="couple-desc">Alappuzha, Kerala</p>
            </div>
        </div>
    </section>
    
    <!-- Wedding Details -->
    <section class="details-section" id="details">
        <div class="details-container">
            <h2 class="section-title">Wedding Details</h2>
            
            <div class="date-time">29 Monday December 2025</div>
            <div class="date-subtext">Time: 10:30 AM</div>
            
            <div class="venue-card">
                <h3 class="venue-name">Holy Matrimony</h3>
                <p class="venue-address">
                    <i class="fas fa-church"></i> St. Mary's Salem Orthodox Church<br>
                    Manappally, Kerala
                </p>
                <p>The sacred union will be solemnized with Holy Qurbana</p>
            </div>
            
            <div class="reception-card">
                <h3 class="venue-name">Reception & Wedding Feast</h3>
                <p class="venue-address">
                    <i class="fas fa-glass-cheers"></i> St. Mary's Salem Parish Hall<br>
                    Manappally, Karunagapally, Kerala
                </p>
                <p>Immediately following the wedding ceremony</p>
            </div>
            
            <a href="https://maps.google.com/?q=St.+Mary's+Salem+Orthodox+Church,+Manappally,+Kerala" target="_blank" class="save-date">
                <i class="fas fa-map-marker-alt"></i> Get Directions
            </a>
        </div>
    </section>
    
    <!-- Map Section -->
    <section class="map-section">
        <div class="map-container">
            <!-- You can embed Google Maps here -->
            <div style="width: 100%; height: 400px; background-color: #f0e8dd; display: flex; align-items: center; justify-content: center; color: #777;">
                <div style="text-align: center;">
                    <i class="fas fa-map-marked-alt" style="font-size: 3rem; margin-bottom: 1rem; color: var(--gold);"></i>
                    <p>Map to St. Mary's Salem Orthodox Church</p>
                    <p>Manappally, Kerala</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Prayer Request -->
    <section class="prayer-section">
        <h2 class="section-title">Your Prayers & Blessings</h2>
        <p class="prayer-text">
            With hearts full of love and gratitude, we joyfully invite you to join us as we exchange our vows and begin our new journey together in Christ.
        </p>
        <p class="prayer-text">
            Your presence and prayers will be our greatest blessing on this special day.
        </p>
        <button class="prayer-btn" onclick="shareBlessing()">
            <i class="fas fa-pray"></i> Send Your Blessings
        </button>
    </section>
    
    <!-- Footer -->
    <footer class="footer">
        <p class="footer-text">Please join us to witness the holy union and celebrate the joy of love and togetherness.</p>
        
        <div class="footer-verse">
            "The Lord bless you and keep you; the Lord make his face shine on you and be gracious to you."<br>
            - Numbers 6:24-25
        </div>
        
        <p class="footer-text">With love,</p>
        <h3 style="font-size: 2rem; color: var(--light-gold); margin: 1rem 0;">Yohannan & Family</h3>
        
        <div class="footer-note">
            <p>Sharing happiness: Aneesh Yohannan</p>
            <p>For any queries, please contact: +91 XXXXX XXXXX</p>
        </div>
        
        <div style="margin-top: 2rem;">
            <i class="fas fa-cross" style="font-size: 2rem; color: var(--light-gold);"></i>
        </div>
    </footer>
    
    <script>
        // Countdown Timer
        const weddingDate = new Date('December 29, 2025 10:30:00').getTime();
        
        function updateCountdown() {
            const now = new Date().getTime();
            const timeLeft = weddingDate - now;
            
            if (timeLeft > 0) {
                const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
                const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);
                
                document.getElementById('days').textContent = days.toString().padStart(2, '0');
                document.getElementById('hours').textContent = hours.toString().padStart(2, '0');
                document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
                document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
            } else {
                document.querySelector('.countdown').innerHTML = '<h3 style="color: white; font-size: 2rem;">Today is the blessed day!</h3>';
            }
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
        
        // Blessing function
        function shareBlessing() {
            const name = prompt("Please enter your name to send your blessings:");
            if (name) {
                const message = prompt(`Thank you, ${name}! Please share your blessing/message for Alex & Shilpa:`);
                if (message) {
                    alert(`Thank you for your beautiful blessing, ${name}! May God bless you abundantly.`);
                    // In a real implementation, you would send this data to a server
                }
            }
        }
        
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
        
        // Add to calendar function
        function addToCalendar() {
            const eventTitle = "Alex & Shilpa's Wedding";
            const eventDate = "20251229T100000";
            const eventLocation = "St. Mary's Salem Orthodox Church, Manappally, Kerala";
            
            // Create ICS file
            const icsContent = `BEGIN:VCALENDAR
VERSION:2.0
BEGIN:VEVENT
SUMMARY:${eventTitle}
DTSTART:${eventDate}
LOCATION:${eventLocation}
DESCRIPTION:Holy Matrimony of Alex Yohannan and Shilpa Shyam
END:VEVENT
END:VCALENDAR`;
            
            const blob = new Blob([icsContent], { type: 'text/calendar' });
            const url = window.URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'Alex-Shilpa-Wedding.ics';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
        }
        
        // Add calendar functionality to save date button
        document.querySelector('.save-date').addEventListener('click', function(e) {
            if (this.getAttribute('href') === '#details') {
                e.preventDefault();
                addToCalendar();
                alert('Wedding details saved to your calendar!');
            }
        });
    </script>
</body>
</html>
