<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Anniversary 💕</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            width: 100%;
            height: 100vh;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            position: relative;
        }

        .container {
            text-align: center;
            z-index: 10;
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            max-width: 600px;
            animation: slideIn 1s ease-out;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            color: #fff;
            font-size: 3em;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
        }

        .subtitle {
            color: #fff;
            font-size: 1.5em;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .message {
            color: #fff;
            font-size: 1.2em;
            margin-bottom: 40px;
            line-height: 1.8;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.3);
        }

        .timer {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .time-unit {
            background: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 10px;
            min-width: 80px;
        }

        .time-unit h2 {
            color: #fff;
            font-size: 2em;
            margin-bottom: 10px;
        }

        .time-unit p {
            color: #ddd;
            font-size: 0.9em;
        }

        .button {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 15px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.1em;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            box-shadow: 0 4px 15px rgba(245, 87, 108, 0.4);
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        .button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(245, 87, 108, 0.6);
        }

        .button:active {
            transform: translateY(0);
        }

        /* Floating Hearts */
        .heart {
            position: absolute;
            width: 30px;
            height: 30px;
            background: #ff6b9d;
            opacity: 0.8;
            animation: float-up 6s ease-in forwards;
            pointer-events: none;
        }

        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            width: 30px;
            height: 48px;
            background: #ff6b9d;
            border-radius: 30px 30px 0 0;
            top: -24px;
            opacity: 0.8;
        }

        .heart::before {
            left: -15px;
            transform: rotate(-45deg);
            transform-origin: 0 24px;
        }

        .heart::after {
            right: -15px;
            transform: rotate(45deg);
            transform-origin: 30px 24px;
        }

        @keyframes float-up {
            0% {
                transform: translateY(0) translateX(0) scale(1);
                opacity: 1;
            }
            50% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) translateX(100px) scale(0);
                opacity: 0;
            }
        }

        .heart:nth-child(1) {
            left: 10%;
            animation-delay: 0s;
            animation-duration: 8s;
        }

        .heart:nth-child(2) {
            left: 20%;
            animation-delay: 1s;
            animation-duration: 7s;
        }

        .heart:nth-child(3) {
            left: 30%;
            animation-delay: 2s;
            animation-duration: 9s;
        }

        .heart:nth-child(4) {
            left: 40%;
            animation-delay: 0.5s;
            animation-duration: 8s;
        }

        .heart:nth-child(5) {
            left: 50%;
            animation-delay: 1.5s;
            animation-duration: 7.5s;
        }

        .heart:nth-child(6) {
            left: 60%;
            animation-delay: 0.8s;
            animation-duration: 9s;
        }

        .heart:nth-child(7) {
            left: 70%;
            animation-delay: 2s;
            animation-duration: 8s;
        }

        .heart:nth-child(8) {
            left: 80%;
            animation-delay: 1s;
            animation-duration: 7.5s;
        }

        .heart:nth-child(9) {
            left: 90%;
            animation-delay: 1.5s;
            animation-duration: 9s;
        }

        @media (max-width: 600px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 2em;
            }

            .subtitle {
                font-size: 1.2em;
            }

            .message {
                font-size: 1em;
            }

            .timer {
                gap: 15px;
            }

            .time-unit {
                min-width: 60px;
                padding: 15px;
            }

            .time-unit h2 {
                font-size: 1.5em;
            }
        }
    </style>
</head>
<body>
    <!-- Animated Hearts Background -->
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>
    <div class="heart"></div>

    <!-- Main Content -->
    <div class="container">
        <h1>💕 Happy Anniversary 💕</h1>
        <p class="subtitle">1 Month Together</p>
        
        <p class="message">
            Every moment with you is a gift.<br>
            Even the distance can't break what we have.<br>
            You make every day special, and I can't wait<br>
            for the day we won't be apart anymore. 💑
        </p>

        <div class="timer">
            <div class="time-unit">
                <h2 id="days">0</h2>
                <p>Days Together</p>
            </div>
            <div class="time-unit">
                <h2 id="hours">0</h2>
                <p>Hours</p>
            </div>
            <div class="time-unit">
                <h2 id="minutes">0</h2>
                <p>Minutes</p>
            </div>
            <div class="time-unit">
                <h2 id="seconds">0</h2>
                <p>Seconds</p>
            </div>
        </div>

        <button class="button" onclick="sendLove()">Send Love 💌</button>
    </div>

    <script>
        // Calculate time since relationship started
        const relationshipStart = new Date('2026-04-25T00:00:00').getTime();

        function updateTimer() {
            const now = new Date().getTime();
            const difference = now - relationshipStart;

            const days = Math.floor(difference / (1000 * 60 * 60 * 24));
            const hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((difference % (1000 * 60)) / 1000);

            document.getElementById('days').textContent = days;
            document.getElementById('hours').textContent = hours;
            document.getElementById('minutes').textContent = minutes;
            document.getElementById('seconds').textContent = seconds;
        }

        // Update timer every second
        updateTimer();
        setInterval(updateTimer, 1000);

        // Send Love Button Animation
        function sendLove() {
            const button = event.target;
            button.style.transform = 'scale(0.95)';
            
            // Create multiple hearts floating up
            for (let i = 0; i < 5; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.className = 'heart';
                    heart.style.left = Math.random() * 100 + '%';
                    heart.style.width = Math.random() * 20 + 20 + 'px';
                    heart.style.height = heart.style.width;
                    document.body.appendChild(heart);
                    
                    setTimeout(() => heart.remove(), 9000);
                }, i * 100);
            }

            // Button feedback
            setTimeout(() => {
                button.style.transform = 'scale(1)';
            }, 100);

            // Alert message
            setTimeout(() => {
                alert('💕 Your love has been sent! 💕\n\nI love you so much! 💑');
            }, 300);
        }

        // Create initial floating hearts
        function createFloatingHearts() {
            setInterval(() => {
                const heart = document.createElement('div');
                heart.className = 'heart';
                heart.style.left = Math.random() * 100 + '%';
                heart.style.width = Math.random() * 15 + 15 + 'px';
                heart.style.height = heart.style.width;
                document.body.appendChild(heart);
                
                setTimeout(() => heart.remove(), 9000);
            }, 1500);
        }

        createFloatingHearts();
    </script>
</body>
</html>
