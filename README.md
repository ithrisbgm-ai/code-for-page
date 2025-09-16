<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>SmartCrop Advisory</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Language Toggle -->
  <div class="lang-toggle">
    <button id="en-btn" class="active">English</button>
    <button id="ta-btn">தமிழ்</button>
  </div>
  
  <!-- Header / Hero Section -->
  <header class="hero">
    <div class="hero-bg"></div>
    <div class="container hero-content">
      <h1 id="app-name">SmartCrop Advisory</h1>
      <p id="tagline">Empowering Farmers with Real-Time Crop Insights</p>
      <div class="cta-buttons">
        <a href="#" class="btn primary">Download App</a>
        <a href="#features" class="btn secondary">Learn More</a>
      </div>
    </div>
    <div class="hero-illustration">
      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="Indian farm fields" />
      <div class="ai-graphic">
        <i class="fas fa-robot fa-3x"></i>
        <span>AI Powered</span>
      </div>
    </div>
  </header>
  
  <!-- Features Section -->
  <section class="features" id="features">
    <div class="container">
      <h2>Main Features</h2>
      <div class="features-grid">
        <div class="feature-card">
          <i class="fas fa-broadcast-tower feature-icon animate"></i>
          <h3>Real-time, location-specific crop advisory</h3>
          <p>Get personalized crop advice based on your farm's exact location and conditions.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-seedling feature-icon animate"></i>
          <h3>Soil health & fertilizer recommendations</h3>
          <p>Receive tailored fertilizer and soil management tips for optimal crop health.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-cloud-sun feature-icon animate"></i>
          <h3>Weather-based alerts and predictions</h3>
          <p>Stay updated with timely weather alerts and forecasts for your region.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-bug feature-icon animate"></i>
          <h3>Pest/disease detection with image uploads</h3>
          <p>Identify crop issues instantly by uploading photos of affected plants.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-rupee-sign feature-icon animate"></i>
          <h3>Market price tracking</h3>
          <p>Track real-time market prices to make informed selling decisions.</p>
        </div>
        <div class="feature-card">
          <i class="fas fa-microphone feature-icon animate"></i>
          <h3>Voice support for low-literacy users</h3>
          <p>Access all features and info using simple voice commands in your language.</p>
        </div>
      </div>
    </div>
  </section>
  
  <!-- Impact Section -->
  <section class="impact">
    <div class="container">
      <h2>Our Impact</h2>
      <p>
        SmartCrop Advisory helps farmers boost productivity, reduce costs, and farm sustainably.
        <br>
        <strong>ICT-based advisories can increase crop yield by 20–30%*</strong>
      </p>
      <ul class="impact-list">
        <li><i class="fas fa-arrow-up"></i> Higher crop yields</li>
        <li><i class="fas fa-leaf"></i> Sustainable farming practices</li>
        <li><i class="fas fa-wallet"></i> Lower input costs</li>
      </ul>
      <small>*Based on agricultural extension research in India.</small>
    </div>
  </section>
  
  <!-- Testimonials Section -->
  <section class="testimonials">
    <div class="container">
      <h2>What Our Users Say</h2>
      <div class="testimonials-grid">
        <div class="testimonial-card">
          <p>"With SmartCrop, I know exactly when to irrigate and what fertilizer to use. My yield has improved a lot!"</p>
          <span>- Ramesh, Farmer, Tamil Nadu</span>
        </div>
        <div class="testimonial-card">
          <p>"The pest detection is amazing. I just take a photo, and get instant advice."</p>
          <span>- Sita, Organic Farmer</span>
        </div>
        <div class="testimonial-card">
          <p>"Our NGO recommends SmartCrop to all the farmers in our network."</p>
          <span>- AgriConnect NGO</span>
        </div>
        <div class="testimonial-card">
          <p>"Accurate weather alerts helped us avoid crop loss during heavy rains."</p>
          <span>- Agricultural Officer, Erode</span>
        </div>
      </div>
    </div>
  </section>
  
  <!-- Call-to-Action & Contact Section -->
  <section class="cta-contact">
    <div class="container cta-contact-flex">
      <div>
        <h2>Ready to Empower Your Farm?</h2>
        <a href="#" class="btn primary">Download App</a>
        <a href="#" class="btn secondary">Join Newsletter</a>
      </div>
      <form class="contact-form">
        <h3>Contact Us</h3>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message"></textarea>
        <button type="submit" class="btn primary">Send</button>
      </form>
    </div>
  </section>
  
  <!-- Footer -->
  <footer>
    <div class="container footer-flex">
      <div>
        <a href="#">About</a> | 
        <a href="#">Contact</a> | 
        <a href="#">Privacy Policy</a>
      </div>
      <div class="footer-social">
        <a href="#"><i class="fab fa-facebook" aria-label="Facebook"></i></a>
        <a href="#"><i class="fab fa-x-twitter" aria-label="Twitter"></i></a>
        <a href="#"><i class="fab fa-youtube" aria-label="YouTube"></i></a>
      </div>
      <div>
        <span>&copy; 2025 SmartCrop Advisory</span>
      </div>
    </div>
  </footer>
  
  <!-- Optional: Simple Animation Script for Feature Icons -->
  <script>
    // Animate feature icons on scroll
    const icons = document.querySelectorAll('.feature-icon');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if(entry.isIntersecting) {
          entry.target.classList.add('show');
        }
      });
    }, { threshold: 0.3 });
    icons.forEach(icon => observer.observe(icon));

    // Language toggle mockup (replace content in real app)
    document.getElementById('en-btn').onclick = function() {
      document.getElementById('app-name').textContent = 'SmartCrop Advisory';
      document.getElementById('tagline').textContent = 'Empowering Farmers with Real-Time Crop Insights';
      this.classList.add('active');
      document.getElementById('ta-btn').classList.remove('active');
    }
    document.getElementById('ta-btn').onclick = function() {
      document.getElementById('app-name').textContent = 'ஸ்மார்ட் கிராப் அறிவுரை';
      document.getElementById('tagline').textContent = 'உண்மையான பயிர் அறிவுரைகளுடன் விவசாயிகளை சக்தி வாய்ந்தவராக்குங்கள்';
      this.classList.add('active');
      document.getElementById('en-btn').classList.remove('active');
    }
  </script>
</body>
</html>
