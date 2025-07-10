<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Motivate with Avocardlo</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f0f4f8;
      color: #333;
    }

    .hero {
      background: linear-gradient(135deg, #4facfe, #00f2fe);
      color: white;
      padding: 100px 20px 60px;
      text-align: center;
    }

    .hero h1 {
      font-size: 4rem;
      font-weight: bold;
    }

    .hero p {
      font-size: 1.3rem;
      margin-top: 20px;
    }

    .section-title {
      margin-top: 60px;
      text-align: center;
      font-size: 2.5rem;
      font-weight: bold;
    }

    .thoughts-section {
      max-width: 1000px;
      margin: 0 auto;
      padding: 40px 20px;
      column-count: 2;
      column-gap: 40px;
    }

    .thought {
      break-inside: avoid;
      background: white;
      margin-bottom: 20px;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.05);
    }

    .instagram-section {
      padding: 60px 20px;
      background: #fff;
      text-align: center;
    }

    .insta-card {
      display: inline-block;
      width: 300px;
      margin: 15px;
      padding: 20px;
      background: #fafafa;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    }

    .insta-card h3 {
      margin-bottom: 10px;
    }

    .insta-btn {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 25px;
      border-radius: 30px;
      background: #ee2a7b;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    footer {
      text-align: center;
      padding: 30px;
      background: #222;
      color: white;
      margin-top: 50px;
    }
  </style>
</head>
<body>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Welcome to Avocardlo Motivation</h1>
    <p>Empowering students with inspiration, knowledge, and positive energy.</p>
  </section>

  <!-- Thoughts Section -->
  <h2 class="section-title">100+ Motivational Thoughts for Students</h2>
  <section class="thoughts-section">
    <!-- Example Thought Cards -->
    <!-- You can generate more below or automate them -->
    <!-- 100+ thoughts inserted below -->
    <script>
      const container = document.currentScript.parentElement;
      const thoughts = [
        "Believe in yourself and all that you are.",
        "Success doesn’t come from what you do occasionally, it comes from what you do consistently.",
        "Discipline is the bridge between goals and accomplishment.",
        "Don’t wait for opportunity. Create it.",
        "Push yourself, because no one else is going to do it for you.",
        "Great things never come from comfort zones.",
        "Dream it. Wish it. Do it.",
        "Wake up with determination. Go to bed with satisfaction.",
        "Little things make big days.",
        "Do something today that your future self will thank you for.",
        "It’s going to be hard, but hard does not mean impossible.",
        "Don’t stop when you’re tired. Stop when you’re done.",
        "The harder you work for something, the greater you’ll feel when you achieve it.",
        "Dream bigger. Do bigger.",
        "Don’t limit your challenges. Challenge your limits.",
        "Sometimes we’re tested not to show our weaknesses, but to discover our strengths.",
        "Success is what comes after you stop making excuses.",
        "Focus on your goal. Don’t look in any direction but ahead.",
        "Your only limit is your mind.",
        "Work hard in silence. Let success make the noise.",
        // Add more up to 100+
      ];

      for (let i = 0; i < 100; i++) {
        const div = document.createElement("div");
        div.className = "thought";
        div.textContent = thoughts[i % thoughts.length];
        container.appendChild(div);
      }
    </script>
  </section>

  <!-- Instagram Section -->
  <h2 class="section-title">Follow Us on Instagram</h2>
  <section class="instagram-section">
    <div class="insta-card">
      <h3>@pk.gihars</h3>
      <p>Inspiration, Growth & Motivation</p>
      <a class="insta-btn" href="https://www.instagram.com/pk.gihars" target="_blank">Follow</a>
    </div>
    <div class="insta-card">
      <h3>@avocardlo</h3>
      <p>Visual vibes and daily motivation</p>
      <a class="insta-btn" href="https://www.instagram.com/avocardlo" target="_blank">Follow</a>
    </div>
    <div class="insta-card">
      <h3>@patnafansclub</h3>
      <p>Student power and Patna pride</p>
      <a class="insta-btn" href="https://www.instagram.com/patnafansclub" target="_blank">Follow</a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Avocardlo Motivation. All rights reserved. | Designed for dreamers & doers.
  </footer>

</body>
</html>
<!-- DARK MODE TOGGLE -->
<button onclick="toggleDarkMode()" style="position:fixed;top:20px;right:20px;padding:8px 12px;border:none;border-radius:5px;background:#333;color:white;z-index:999;">
  🌓 Dark Mode
</button>
<script>
  function toggleDarkMode() {
    document.body.classList.toggle("dark-mode");
  }
</script>
<style>
  .dark-mode {
    background-color: #121212;
    color: #f0f0f0;
  }
  .dark-mode .thought {
    background: #1e1e1e;
    color: #ddd;
  }
</style>
<!-- QUOTE SUBMISSION FORM -->
<section style="padding:40px;text-align:center;">
  <h2>Submit Your Own Quote</h2>
  <form onsubmit="handleQuoteSubmit(event)" style="max-width:500px;margin:auto;">
    <textarea id="quoteInput" placeholder="Write your motivational quote..." required rows="4" style="width:100%;padding:10px;border-radius:10px;"></textarea>
    <br><br>
    <input type="text" id="quoteAuthor" placeholder="Your Name (optional)" style="width:100%;padding:8px;border-radius:10px;">
    <br><br>
    <button type="submit" style="padding:10px 30px;border:none;border-radius:30px;background:#00b894;color:white;">Submit</button>
  </form>
  <div id="thankYouMsg" style="margin-top:20px;color:green;display:none;">Thanks! Your quote was submitted.</div>
</section>

<script>
  function handleQuoteSubmit(e) {
    e.preventDefault();
    document.getElementById("thankYouMsg").style.display = "block";
    // You can later connect this to Firebase, Airtable, or save to backend
    document.getElementById("quoteInput").value = '';
    document.getElementById("quoteAuthor").value = '';
  }
</script>
<!-- INSTAGRAM EMBED SECTION -->
<section style="padding:60px 20px;text-align:center;background:#fff;">
  <h2>Our Instagram – <a href="https://www.instagram.com/avocardlo" target="_blank">@avocardlo</a></h2>
  <iframe src="https://www.instagram.com/p/CwMTlZ-Bbq3/embed" width="400" height="480" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
</section>

