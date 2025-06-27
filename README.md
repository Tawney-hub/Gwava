<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>STRANGERS IN PROXIMITY</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Import Google Fonts for futuristic and clean typography */
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@700&family=Roboto:wght@300;400;700&display=swap');
        /* 'Orbitron' for the title, 'Roboto' for body text */

        :root {
            /* Define your color scheme as CSS variables for easy management */
            --dark-base: #1a1a2e; /* Dark navy/black */
            --accent-cyan: #00ffff;
            --accent-blue: #007bff;
            --accent-red: #ff4500;
            --text-white: #ffffff;
            --text-green: #00ff00; /* Added green for specific elements as requested */
            --glow-color: rgba(0, 255, 255, 0.5); /* Cyan glow for general elements */
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Roboto', sans-serif;
            color: var(--text-white);
            background-color: var(--dark-base); /* Dark base for the background */
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            min-height: 100vh; /* Make sure it takes full viewport height */
            overflow: hidden; /* Hide any overflow from background effects */
            position: relative; /* For positioning absolute elements like background image */
            /* Add a subtle overall glow to the body */
            box-shadow: inset 0 0 50px rgba(0, 255, 0, 0.1); /* Soft green inner glow */
        }

        /* --- Background Image/Effect Container --- */
        .background-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            /*
             * IMPORTANT: Replace 'your-dark-cityscape-or-abstract-signal-map-image.jpg'
             * with the actual path or URL to your background image.
             * This image should be dark, abstract, and have blue/purple tones.
             */
            background: url('https://via.placeholder.com/1920x1080/100020/000000?text=Abstract+Signal+Map') no-repeat center center / cover;
            opacity: 0.5; /* Adjust opacity for a subtle background */
            z-index: -1; /* Ensure it stays behind content */
            filter: brightness(0.7) contrast(1.2); /* Enhance the dark, glowing feel */
            animation: backgroundPulse 10s infinite alternate; /* Subtle breathing animation */
        }

        @keyframes backgroundPulse {
            0% { filter: brightness(0.7) contrast(1.2); }
            100% { filter: brightness(0.8) contrast(1.3); }
        }

        /* --- Main Title Section --- */
        .title-section {
            text-align: center;
            padding: 50px 20px 20px;
            z-index: 1; /* Bring to front */
            /* Added a subtle background for readability against a busy background */
            background: linear-gradient(to bottom, rgba(26, 26, 46, 0.7), rgba(26, 26, 46, 0.3));
            border-bottom: 2px solid var(--accent-cyan);
            width: 100%;
            box-sizing: border-box; /* Include padding in width */
        }

        .main-title {
            font-family: 'Orbitron', sans-serif; /* Glitchy digital font */
            font-size: 5em; /* Large font size */
            color: var(--accent-cyan); /* Cyan for the main title */
            font-weight: 700;
            letter-spacing: 5px;
            text-shadow: 0 0 15px var(--accent-cyan), 0 0 25px var(--accent-cyan);
            animation: glitch 1.5s infinite; /* Glitch effect */
            margin: 0; /* Remove default margins */
        }

        .main-title:last-of-type { /* Style for "A Story Beyond the Signal" */
            font-size: 0.7em; /* Smaller than main title */
            display: block; /* Ensures it's on its own line */
            margin-top: 10px;
            letter-spacing: 2px;
            color: var(--text-green); /* "Story Beyond the Signal" in green */
            text-shadow: 0 0 10px var(--text-green), 0 0 20px var(--text-green);
        }

        .subheading-hook {
            font-size: 1.5em;
            font-style: italic;
            color: var(--text-white);
            margin-top: 15px;
            opacity: 0.8;
        }

        /* Keyframes for a simple glitch effect */
        @keyframes glitch {
            0% { transform: translate(0); text-shadow: 0 0 15px var(--accent-cyan), 0 0 25px var(--accent-cyan); }
            20% { transform: translate(-2px, 2px); text-shadow: 0 0 10px var(--accent-cyan), 0 0 20px var(--accent-blue); }
            40% { transform: translate(-1px, -1px); text-shadow: 0 0 12px var(--accent-blue), 0 0 22px var(--accent-cyan); }
            60% { transform: translate(2px, 1px); text-shadow: 0 0 14px var(--accent-cyan), 0 0 24px var(--accent-red); }
            80% { transform: translate(1px, -2px); text-shadow: 0 0 16px var(--accent-red), 0 0 26px var(--accent-cyan); }
            100% { transform: translate(0); text-shadow: 0 0 15px var(--accent-cyan), 0 0 25px var(--accent-cyan); }
        }

        /* --- Foreground Image Section (Placeholder) --- */
        .foreground-image-section {
            position: relative;
            width: 80%; /* Adjust as needed */
            max-width: 800px; /* Max width for the image */
            margin: 40px auto;
            z-index: 2; /* Ensure it's above background */
            aspect-ratio: 16 / 9; /* Maintain aspect ratio (e.g., for a video call image) */
            background: url('https://via.placeholder.com/800x450/000000/00ffff?text=Two+People+Video+Chatting') no-repeat center center / contain;
            /* IMPORTANT: Replace with your actual image of two people on phone screens.
             * Make sure the image is transparent or has a dark background to blend well.
             */
            filter: drop-shadow(0 0 25px var(--glow-color)); /* Soft cyan glow around the image */
            border: 2px solid var(--accent-cyan); /* Border to simulate screen edge */
            animation: imagePulse 3s infinite alternate; /* Subtle image pulse */
        }

        @keyframes imagePulse {
            0% { transform: scale(1); filter: drop-shadow(0 0 25px var(--glow-color)); }
            100% { transform: scale(1.01); filter: drop-shadow(0 0 35px var(--glow-color)); }
        }

        /* --- Overlay Visual Additions (Simulated for demonstration) --- */
        /* These are best integrated into your generated image for realism. */
        /* If you want actual CSS ripples or sound waves, you'd add more divs */
        /* and apply animation to them, positioned absolutely over the image. */

        /* Example of a simulated ripple/soundwave around the image section */
        .foreground-image-section::before,
        .foreground-image-section::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            border-radius: 50%;
            border: 2px solid;
            animation: ripple 2.5s infinite ease-out;
            pointer-events: none; /* Allows clicks through */
        }

        .foreground-image-section::before {
            width: 110%;
            height: 110%;
            border-color: var(--accent-red); /* Red sound wave */
            animation-delay: 0s;
        }

        .foreground-image-section::after {
            width: 120%;
            height: 120%;
            border-color: var(--text-green); /* Green sound wave */
            animation-delay: 1.25s; /* Stagger the animation */
        }

        @keyframes ripple {
            0% { transform: translate(-50%, -50%) scale(0.8); opacity: 0.7; }
            100% { transform: translate(-50%, -50%) scale(1.2); opacity: 0; }
        }


        /* --- Contact Section --- */
        .contact-section {
            text-align: center;
            padding: 25px;
            background-color: rgba(0, 0, 0, 0.6); /* Slightly more opaque background */
            border-top: 2px solid var(--accent-cyan);
            width: 100%;
            box-sizing: border-box; /* Include padding in width */
            z-index: 1; /* Bring to front */
            box-shadow: 0 -5px 20px rgba(0, 255, 0, 0.1); /* Soft green shadow at the top */
        }

        .contact-section h3 {
            color: var(--accent-cyan);
            font-size: 1.4em;
            margin-bottom: 20px;
            text-shadow: 0 0 10px var(--accent-cyan);
        }

        .channel-info {
            display: flex;
            justify-content: center;
            gap: 40px; /* More space between channels */
            flex-wrap: wrap;
            margin-bottom: 25px;
        }

        .channel {
            display: flex;
            align-items: center;
            gap: 12px;
            color: var(--text-white);
            font-size: 1.2em;
            text-decoration: none; /* Remove underline from links */
            padding: 10px 15px;
            border: 1px solid var(--accent-blue);
            border-radius: 5px;
            background-color: rgba(0, 50, 100, 0.3);
            transition: all 0.3s ease;
            box-shadow: 0 0 10px rgba(0, 255, 0, 0.2); /* Green glow on channels */
        }

        .channel:hover {
            color: var(--text-green); /* Green on hover */
            border-color: var(--text-green);
            background-color: rgba(0, 100, 50, 0.5);
            transform: translateY(-3px);
            box-shadow: 0 0 15px rgba(0, 255, 0, 0.4), 0 0 25px rgba(0, 255, 0, 0.2);
        }

        .channel .icon {
            font-size: 1.8em;
            color: var(--text-green); /* Icons in green */
            margin-right: 5px;
        }

        .phone-number {
            font-size: 1.6em;
            font-weight: bold;
            color: var(--text-green); /* Phone number in green */
            margin-top: 15px;
            text-shadow: 0 0 15px var(--text-green), 0 0 25px var(--text-green);
            letter-spacing: 1px;
            animation: neonPulse 2s infinite alternate;
        }

        @keyframes neonPulse {
            0% { text-shadow: 0 0 10px var(--text-green), 0 0 20px var(--text-green); }
            100% { text-shadow: 0 0 15px var(--text-green), 0 0 30px var(--text-green), 0 0 40px rgba(0, 255, 0, 0.5); }
        }

        /* --- Responsive Design --- */
        @media (max-width: 992px) {
            .main-title {
                font-size: 4em;
            }
            .main-title:last-of-type {
                font-size: 0.6em;
            }
            .subheading-hook {
                font-size: 1.3em;
            }
            .foreground-image-section {
                width: 90%;
            }
        }

        @media (max-width: 768px) {
            .main-title {
                font-size: 3em;
            }
            .main-title:last-of-type {
                font-size: 0.5em;
            }
            .subheading-hook {
                font-size: 1.1em;
            }
            .foreground-image-section {
                height: 300px; /* Adjust if aspect-ratio doesn't suffice */
                width: 95%;
            }
            .channel-info {
                flex-direction: column;
                gap: 20px;
            }
            .channel {
                font-size: 1.1em;
            }
            .channel .icon {
                font-size: 1.6em;
            }
            .phone-number {
                font-size: 1.4em;
            }
        }

        @media (max-width: 480px) {
            .main-title {
                font-size: 2.2em;
                letter-spacing: 2px;
            }
            .main-title:last-of-type {
                font-size: 0.45em;
            }
            .subheading-hook {
                font-size: 0.9em;
            }
            .foreground-image-section {
                height: 200px;
                margin: 20px auto;
            }
            .contact-section {
                padding: 15px;
            }
            .channel {
                padding: 8px 10px;
            }
            .phone-number {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>
    <div class="background-container"></div>

    <header class="title-section">
        <h1 class="main-title">STRANGERS IN PROXIMITY</h1>
        <h2 class="main-title">A Story Beyond the Signal</h2>
        <p class="subheading-hook">Some faces aren’t random. They’re chosen.</p>
    </header>

    <main class="foreground-image-section">
        </main>

    <footer class="contact-section">
        <h3>📱 Join the Viba Team & Get App Updates</h3>
        <div class="channel-info">
            <a href="https://wa.me/message/YOUR_WHATSAPP_CHANNEL_LINK_HERE" target="_blank" class="channel">
                <span class="icon fab fa-whatsapp"></span> WhatsApp Channel: Viba App Releases
            </a>
            <a href="https://t.me/YOUR_TELEGRAM_CHANNEL_LINK_HERE" target="_blank" class="channel">
                <span class="icon fab fa-telegram-plane"></span> Telegram Channel: Viba App Releases
            </a>
        </div>
        <p class="phone-number">Contact: 0780297586</p>
        </footer>
</body>
</html>