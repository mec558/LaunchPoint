<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LaunchPoint</title>
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #062437;
            color: #fff;
            min-height: 100vh;
        }

        /* Navigation */
        .nav {
            display: flex;
            justify-content: center;
            background-color: #b93906;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav button {
            background: none;
            border: none;
            color: #000000;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            transition: color 0.3s;
        }

        .nav button:hover, .nav button.active {
            color: #e53935;
        }

        

        /* Sections */
        .section {
            display: none;
            padding: 60px 20px;
            max-width: 900px;
            margin: auto;
        }

        .section.active {
            display: block;
        }

        /* Home Logo */
        .home-logo {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 30px;
        }

        
        

        .home-logo h1 {
            font-size: 48px;
            color: #fff9f9;
            margin-bottom: 10px;
        }

        /* Home Article */
        .home-article {
            font-size: 18px;
            line-height: 1.7;
        }

        .highlight {
            color: #ca2525;
            cursor: pointer;
            text-decoration: underline;
        }

        /* Get Website */
        .get-website, .get-flyers, .get-social {
            width : 100%;
            background-color: #1a1a1a;
            border-radius: 8px;
            border: 2px solid #a11f1f;
            
            border-color: #b93906;
            max-width: 700px;
            margin: auto;
        }
.get-website {
            background-color: #1a1a1a;
            color: #fff;
            border: 2px solid #b93906;
        }
        .get-website {
            background-color: #005bf900;
            color: #fcfcfc;
        }   

        .get-website h2 {
            color: #0188f6;
            margin-bottom: 15px;
        }

        .get-website ul {
            margin: 15px 0 20px 20px;
        }

        .get-website button {
            background-color: #039520;
            border: 10px solid #77ed92;
            padding: 12px 20px;
            color: #181616;
            cursor: pointer;
            font-size: 16px;
            border-radius: 4px;
        }

        /* Get Flyers */
        .get-flyers {
            background-color:#062437;
            color: #fff;
            border: 2px solid #b93906;
        }

        .get-flyers h2 {
            color: #0188f6;
            margin-bottom: 15px;
        }

        .get-flyers input, .get-flyers textarea {
            width: 100%;
            padding: 70px;
            margin-bottom: 12px;
            border: 1px solid #ff5252;
            border-radius: 5px;
            background-color: #111;
            color: #fff;
        }

        .get-flyers button {
            background-color: #06b32c;
            border: none;
            padding: 12px 20px;
            color: #fff;
            cursor: pointer;
            font-size: 16px;
            border-radius: 4px;
        }

        /* Get Social */
        .get-social {
            background-color: #062437;
            color: #fff;
        }

        .get-social h2 {
            color: #0188f6;
            margin-bottom: 15px;
        }

        .get-social input, .get-social textarea, .get-social select {
            width: 100%;
            padding: 10px;
            margin-bottom: 12px;
            border: 1px solid #42a5f5;
            border-radius: 5px;
            background-color: #b93906;
            color: #fff;
        }

        .get-social button {
            background-color: #0bc43c;
            border: none;
            padding: 12px 20px;
            color: #fff;
            cursor: pointer;
            font-size: 16px;
            border-radius: 4px;
        }

        /* Links */
        a {
            color: inherit;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

    </style>
</head>
<body>

    <!-- Navigation -->
    <div class="nav">
        <button class="tab-btn active" data-tab="home">Home</button>
        <button class="tab-btn" data-tab="website">Get Website</button>
        <button class="tab-btn" data-tab="flyers">Get Flyers</button>
        <button class="tab-btn" data-tab="social">Get Social Account</button>
    </div>

    <!-- Help Menu -->
    <div class="help-menu" onclick="alert('Navigate by clicking the tabs on top. Click highlights on Home to go to services.');">
        
    </div>

    <!-- Home Section -->
    <div id="home" class="section active">
        <div class="home-logo">
            
            <h1>Launch<span class="highlight">Point</span></h1>
            <h2 style="align-self:flex-start; margin-top:10px;">What LaunchPoint Offers</h2>
        </div>
        <div class="home-article">
            LaunchPoint is a professional company helping businesses grow digitally and visually. We specialize in <span class="highlight" onclick="openTab('website')">Website Development</span>, <span class="highlight" onclick="openTab('flyers')">Flyer & Visual Design</span>, and <span class="highlight" onclick="openTab('social')">Social Media Account Setup</span>. Each service is handled by a dedicated specialist, ensuring quality, clarity, and efficiency. We give you our best on every aspect we cover, with the cheapest price possible. We are here to help you get your business up and running with a strong online presence and eye-catching visuals. Whether you need a sleek website, attention-grabbing flyers, or a solid social media foundation, LaunchPoint has got you covered. Let's work together to bring your vision to life and make your business stand out in the digital world.
        </div>
    </div>

    <!-- Get Website -->
    <div id="website" class="section get-website">
        <h2>Ready to turn your idea into a website?</h2>
        <p>LaunchPoint creates professional websites for businesses and also just any website at a <u><strong>one-time payment of $24.99</strong></u>. Delivery time will be discussed directly in the messages after contact.</p>
        <h3>To get started, please make sure to have the required information ready:</h3>
        <ul>
            <li>Business Name</li>
            <li>Logo (if available)</li>
            <li>Description of offerings</li>
            <li>Preferred colors for the website</li>
            <li>Any specific structure or layout requirements</li>
        </ul>
        <button onclick="window.location.href='sms:5593168075?body=Hey LaunchPoint, Can I get a website with... (describe how you want it)'">PROCEED</button>
    </div>

    <!-- Get Flyers -->
    <div id="flyers" class="section get-flyers">
        <h2>Ready to make your idea seen by many?</h2>
        <p>LaunchPoint is ready to make that happen with only <strong>$5</strong> + <strong>$3 per 10 copies</strong> if you need physical copies. Delivery timeline will be discussed via messaging.</p>
        <h3>To get started, please provide the following details:</h3>
    <ul>
        <li>What is the flyer about?</li>
        <li>What should be on the flyer? (QR code, Logo, etc.)</li>
        <li>Preferred colors</li>
        <li>Anything else you want on the flyer?</li>
    </Ul>

    
        <button onclick="window.location.href='https://www.instagram.com/__ramosir/'">Let's Get the Flier</button>

    </div>

    <!-- Get Social Account -->
    <div id="social" class="section get-social">
        <h2>Ready to grow your presence online?</h2>
        <p>Social Media are some of the most important tools a bussines needs to get going ( Not just to be famous but to get people aware of them) .LaunchPoint will set up your social media accounts for you with a payment of only <strong>$10</strong>. Timeline will be communicated in messaging.</p>
        <h3>To get started, please provide the following details:</h3>
        <ul>
            <li>Platform(s) required</li>
            <li>Business name / handle preferences</li>
            <li>Logo / branding materials</li>
            <li>Content focus</li>
            <li>Account registration preference (email or phone)</li>
            <li>Special instructions / themes</li>
        </ul>
        <button onclick="window.location.href='sms:5592463134?body=Hey LaunchPoint, I’d like to set up social media accounts for... (platforms / details)'">Let's Set Up My Social Account</button>
    </div>

    <!-- Scripts -->
    <script>
        const tabs = document.querySelectorAll('.tab-btn');
        const sections = document.querySelectorAll('.section');

        tabs.forEach(tab => {
            tab.addEventListener('click', () => {
                tabs.forEach(btn => btn.classList.remove('active'));
                tab.classList.add('active');

                const target = tab.getAttribute('data-tab');
                sections.forEach(sec => sec.classList.remove('active'));
                document.getElementById(target).classList.add('active');
            });
        });

        function openTab(tabId) {
            document.querySelector(`.tab-btn[data-tab=${tabId}]`).click();
        }
    </script>

</body>
</html>
