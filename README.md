# website

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Badarriyya Catering Service</title>
  <style>
    /* Reset & base */
    body, h1, h2, h3, p, ul, li, a, input, button {
      margin: 0; padding: 0; box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      background: #fff3e0;
      color: #4d2600;
      line-height: 1.6;
    }
    a {
      color: #d32f2f;
      text-decoration: none;
      transition: color 0.3s;
    }
    a:hover {
      color: #ff6600;
    }

    /* Header */
    header {
      position: sticky;
      top: 0;
      background: linear-gradient(90deg, #ff4d4d, #ffa500, #ffff66);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      color: #fff;
      z-index: 999;
    }
    header .logo {
      font-size: 1.8rem;
      font-weight: 700;
      display: flex;
      align-items: center;
      gap: 10px;
    }
    header .logo span {
      font-size: 1.4rem;
    }
    nav {
      display: flex;
      gap: 25px;
    }
    nav a {
      font-weight: 600;
      font-size: 1rem;
      color: #d32f2f;
      background: #fff3e0;
      padding: 8px 12px;
      border-radius: 5px;
    }
    nav a:hover {
      background: #ff4d4d;
      color: #fff;
    }

    /* Contact info */
    .contact-info {
      display: flex;
      gap: 25px;
      font-size: 0.9rem;
      font-weight: 600;
      color: #fff;
    }
    .contact-info a {
      color: #fff;
    }
    .contact-info a:hover {
      color: #ffff66;
    }

    /* Hero Section */
    .hero {
      background: url('https://images.unsplash.com/photo-1543352634-11bcdc9f96d0?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
      height: 400px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #fff;
      padding: 0 20px;
    }
    .hero h1 {
      font-size: 3rem;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.7);
      margin-bottom: 15px;
    }
    .hero p {
      font-size: 1.3rem;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.6);
      margin-bottom: 30px;
      max-width: 600px;
    }
    .hero .btn {
      background: #ffff66;
      color: #d32f2f;
      border: none;
      padding: 12px 30px;
      font-weight: 700;
      font-size: 1.1rem;
      border-radius: 30px;
      cursor: pointer;
      margin: 5px;
      transition: background 0.3s;
      box-shadow: 0 4px 8px rgba(255, 165, 0, 0.5);
      text-decoration: none;
      display: inline-block;
    }
    .hero .btn:hover {
      background: #ff6600;
      color: #fff;
    }

    /* Sections */
    section {
      max-width: 1000px;
      margin: 60px auto;
      padding: 0 20px;
    }
    section h2 {
      color: #d32f2f;
      margin-bottom: 20px;
      font-size: 2.2rem;
      border-bottom: 3px solid #ffa500;
      display: inline-block;
      padding-bottom: 5px;
    }

    /* About */
    #about p {
      font-size: 1.1rem;
      color: #4d2600;
      max-width: 800px;
      margin: auto;
      line-height: 1.7;
    }

    /* Services */
    #services ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 25px;
      justify-content: center;
    }
    #services li {
      background: #fff3e0;
      border: 2px solid #ffa500;
      border-radius: 12px;
      padding: 20px 25px;
      font-size: 1.1rem;
      font-weight: 600;
      flex: 1 1 200px;
      text-align: center;
      box-shadow: 0 4px 6px rgba(255, 165, 0, 0.3);
      transition: transform 0.3s ease;
      cursor: default;
    }
    #services li:hover {
      transform: scale(1.05);
      border-color: #ff4d4d;
      box-shadow: 0 8px 10px rgba(255, 77, 77, 0.5);
    }

    /* Testimonials */
    #testimonials {
      background: #ff4d4d;
      color: #fff;
      padding: 40px 20px;
      border-radius: 15px;
      max-width: 900px;
      margin: 60px auto;
      box-shadow: 0 8px 15px rgba(255, 77, 77, 0.4);
    }
    #testimonials blockquote {
      font-style: italic;
      font-size: 1.2rem;
      margin-bottom: 25px;
      position: relative;
      padding-left: 25px;
    }
    #testimonials blockquote::before {
      content: "“";
      font-size: 3rem;
      color: #ffff66;
      position: absolute;
      left: 0;
      top: -10px;
    }
    #testimonials footer {
      font-weight: 700;
      font-size: 1rem;
      text-align: right;
    }

    /* Contact */
    #contact form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    #contact label {
      font-weight: 600;
      color: #4d2600;
    }
    #contact input, #contact textarea {
      padding: 10px;
      border: 2px solid #ffa500;
      border-radius: 8px;
      font-size: 1rem;
      resize: vertical;
    }
    #contact button {
      background: #ff4d4d;
      color: #fff;
      font-weight: 700;
      padding: 12px 0;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-size: 1.1rem;
      transition: background 0.3s;
      box-shadow: 0 4px 8px rgba(255, 77, 77, 0.6);
    }
    #contact button:hover {
      background: #d32f2f;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px 0;
      background: #fff3e0;
      font-size: 0.9rem;
      color: #4d2600;
      margin-top: 50px;
    }

    /* Responsive */
    @media(max-width: 768px) {
      nav {
        flex-wrap: wrap;
        justify-content: center;
      }
      header {
        flex-direction: column;
        gap: 10px;
        padding: 15px 15px;
      }
      .contact-info {
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
      }
      .hero h1 {
        font-size: 2.2rem;
      }
      .hero p {
        font-size: 1.1rem;
      }
      #services ul {
        flex-direction: column;
        gap: 15px;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">🍽️ Badarriyya Catering Service</div>
  <nav>
    <a href="#home">Home</a>
    <a href="#services">Menu</a>
    <a href="#events">Events</a>
    <a href="#about">About</a>
    <a href="#testimonials">Testimonials</a>
    <a href="#contact">Contact</a>
  </nav>
  <div class="contact-info" style="display:none;">
    <a href="tel:+918606221010">📞 8606221010</a>
    <span>📍 Malappuram, Kerala</span>
    <a href="mailto:khadersbadariyya@gmail.com">✉️ Email</a>
  </div>
</header>

<section class="hero" id="home">
  <h1>Delicious, Elegant Catering for Every Occasion</h1>
  <p>Serving weddings, corporate events, and private parties across Kerala</p>
  <a href="tel:+918606221010" class="btn">📞 Call Now</a>
  <a href="#contact" class="btn">Get a Free Quote</a>
</section>

<section id="about">
  <h2>About Badarriyya Catering</h2>
  <p>
    We specialize in fresh, flavorful, and beautifully presented cuisine
****
