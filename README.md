# empowering-farmers-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Empowering Farmers - Hackathon Winner</title>
  
  <!-- Importing fonts -->
 
  <style>
    /* Global Styles */
    * {
      
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Roboto', Arial, sans-serif;
      background-image: url('farmers working in the field.png'); /* Replace 'your-image.jpg' with your image's path */;
      color: #333;
      line-height: 1.6;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    
    /* Enhanced Header Styling */
header {
   background-image: url('farmers working in the field.png'); /* Replace 'your-image.jpg' with your image's path */;
  color: white;
  padding: 2rem 1.5rem;
  text-align: center;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  border-radius: 0.5rem;
}

header h1 {
  font-size: 2.5rem;
  font-weight: bold;
  letter-spacing: 2px;
  text-transform: uppercase;
  margin: 0;
}

header p {
  font-size: 1.2rem;
  font-style: italic;
  margin-top: 0.8rem;
  opacity: 0.9;
}


    /* Elevated Tab Navigation */
nav.tab-menu {
  background: linear-gradient(135deg, hwb(216 23% 11%), #444);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
  border-radius: 0.5rem;
  padding: 0.5rem 0;
}

.tab-header {
  display: flex;
  justify-content: center;
  list-style: none;
  margin: 0;
  padding: 0;
}

.tab-header li {
  padding: 1rem 2rem;
  cursor: pointer;
  color: #f5f5f5;
  font-weight: bold;
  font-size: 1rem;
  border-radius: 0.5rem;
  margin: 0 0.5rem;
  transition: all 0.3s ease-in-out;
}

.tab-header li:hover,
.tab-header li.active {
  background: linear-gradient(135deg, #4caf50, #2e7d32);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  color: #ffffff;
  transform: scale(1.05);
}

    /* Refined Tab Content Container */
.tab-content-container {
  padding: 2.5rem;
  background: linear-gradient(145deg, #ffffff, #f4f4f4);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15), inset 0 -1px 2px rgba(0, 0, 0, 0.1);
  margin: 2.5rem auto;
  max-width: 1000px;
  border-radius: 1rem;
  min-height: 65vh;
  border: 1px solid #e0e0e0;
}

.tab-content {
  display: none;
  animation: fadeIn 0.8s cubic-bezier(0.4, 0, 0.2, 1);
  color: #333;
  font-size: 1.1rem;
  line-height: 1.6;
}

.tab-content.active {
  display: block;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(15px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

    /* Refined Content Styles for Each Tab */
.tab-content h2 {
  text-align: center;
  margin-bottom: 1.5rem;
  position: relative;
  font-size: 2rem;
  color: #333;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
}

.tab-content h2::after {
  content: "";
  width: 80px;
  height: 4px;
  background: linear-gradient(90deg, #4caf50, #81c784);
  display: block;
  margin: 1rem auto 0;
  border-radius: 2px;
}

.tab-content p,
.tab-content ul {
  max-width: 750px;
  margin: 1rem auto 1.5rem;
  font-size: 1.2rem;
  line-height: 1.7;
  color: #555;
  text-align: justify;
}

.tab-content ul {
  list-style: none;
  padding: 0;
}

.tab-content ul li {
  margin: 1rem 0;
  padding: 0.5rem 0.5rem 0.5rem 2rem;
  position: relative;
  background: #f9f9f9;
  border-radius: 0.5rem;
  transition: transform 0.3s ease, background 0.3s ease;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.tab-content ul li:hover {
  background: #e8f5e9;
  transform: translateX(5px);
}

.tab-content ul li::before {
  content: "•";
  position: absolute;
  left: 15px;
  font-size: 1.5rem;
  color: #4caf50;
  font-weight: bold;
}

    /* Contact Form Styles */
form {
  max-width: 600px;
  margin: 2rem auto;
  padding: 1.5rem;
  background: #ffffff;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border: 1px solid #e0e0e0;
}

form label {
  display: block;
  margin-bottom: 0.7rem;
  font-size: 1.1rem;
  font-weight: bold;
  color: #555;
}

form input,
form textarea {
  width: 100%;
  padding: 1rem;
  margin-bottom: 1.5rem;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 1rem;
  background: #f9f9f9;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

form input:focus,
form textarea:focus {
  border-color: #4caf50;
  box-shadow: 0 0 6px rgba(76, 175, 80, 0.5);
  outline: none;
}

form button {
  background: linear-gradient(135deg, #4caf50, #43a047);
  color: white;
  border: none;
  padding: 1rem 2rem;
  border-radius: 6px;
  font-size: 1.1rem;
  font-weight: bold;
  cursor: pointer;
  display: block;
  margin: 1rem auto;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
}

form button:hover {
  background: linear-gradient(135deg, #45a049, #388e3c);
  transform: translateY(-2px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
}

form button:active {
  background: linear-gradient(135deg, #388e3c, #2e7d32);
  transform: translateY(1px);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

    /* Enhanced Footer */
footer {
  background: linear-gradient(135deg, #333, #444);
  color: #f5f5f5;
  text-align: center;
  padding: 2rem;
  margin-top: 3rem;
  border-radius: 10px 10px 0 0;
  box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.2);
}

footer p {
  margin-bottom: 1rem;
  font-size: 1.1rem;
  opacity: 0.9;
}

footer a {
  color: #81c784;
  margin: 0 1rem;
  font-weight: bold;
  text-decoration: none;
  transition: color 0.3s ease, transform 0.3s ease;
}

footer a:hover {
  text-decoration: underline;
  color: #4caf50;
  transform: scale(1.1);
}

 /* Enhanced Responsive Styles */
@media (max-width: 768px) {
  .tab-header {
    flex-wrap: wrap;
    gap: 0.8rem;
    justify-content: center;
    padding: 1rem;
    background: linear-gradient(135deg, #f4f4f4, #e0e0e0);
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  .tab-header li {
    padding: 1rem 1.5rem;
    font-size: 0.9rem;
    font-weight: bold;
    background: #ffffff;
    color: #333;
    border: 1px solid #ccc;
    border-radius: 6px;
    transition: all 0.3s ease-in-out;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  .tab-header li:hover {
    background: linear-gradient(135deg, #4caf50, #43a047);
    color: white;
    transform: scale(1.05);
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  }

  .tab-header li.active {
    background: linear-gradient(135deg, #43a047, #388e3c);
    color: white;
    border: none;
    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
  }
}

  </style>
</head>
<body>
    
  <!-- Header Section -->
  <header>
    <h1>Empowering Small & Marginal Farmers</h1>
    <p>Revolutionizing Agriculture with AI-Driven Solutions</p>
  </header>
  <!-- Tab Navigation -->
  <nav class="tab-menu">
    <ul class="tab-header">
    <li><a href="login.html" style="color: #4CAF50; text-decoration: underline;">Login</a></li>
    <li data-tab="overview" class="active">Overview</li>
    <li data-tab="crisis">The Crisis</li>
    <li data-tab="ai-solution">AI Solutions</li>
    <li data-tab="statistics">Statistics</li>
    <li data-tab="stories">Success Stories</li>
    <li data-tab="resources">Resources & Tips</li>
    
    </ul>
  </nav>
  <div class="tab-content-container">
    <div id="overview" class="tab-content active">
      <h2>Overview</h2>
      <p>Welcome to Empowering Farmers, a platform where technology meets tradition. Our mission is to create a smarter, more sustainable future for India's small and marginal farmers through advanced AI solutions.</p>
      <p>Explore the tabs to learn about the crisis facing our farmers, our innovative solutions, data-backed insights, and inspiring success stories.</p>
    </div>

  <div id="crisis" class="tab-content">
      <h2>The Crisis</h2>
      <p>India is home to 126 million small and marginal farmers who face severe challenges:</p>
      <ul>
        <li><strong>Climate Change Impacts:</strong> Unpredictable weather and extreme climatic events.</li>
        <li><strong>Resource Limitations:</strong> Insufficient access to quality seeds, fertilizers, and modern equipment.</li>
        <li><strong>Soil Degradation:</strong> Declining fertility due to unsustainable farming practices.</li>
      </ul>
      <p>These challenges threaten not only individual livelihoods but also the overall food security of the nation.</p>
    </div>

  <div id="ai-solution" class="tab-content">
      <h2>AI Solutions</h2>
      <p>We are harnessing the power of artificial intelligence to empower farmers:</p>
      <ul>
        <li><strong>Real-Time Insights:</strong> Advanced sensors and machine learning models monitor weather patterns and soil health.</li>
        <li><strong>Smart Resource Management:</strong> Customized recommendations for seeds, fertilizers, and irrigation practices.</li>
        <li><strong>Remote Assistance:</strong> AI chatbots available in multiple regional languages to support farmers at every step.</li>
      </ul>
    </div>

  <div id="statistics" class="tab-content">
      <h2>Statistics & Insights</h2>
      <p>Our data-driven approach has already delivered remarkable outcomes:</p>
      <ul>
        <li><strong>Yield Increase:</strong> Farmers report up to a 50% improvement in crop yield.</li>
        <li><strong>Cost Reduction:</strong> Strategic resource management has cut input costs by 30%.</li>
        <li><strong>Adoption Rate:</strong> Over 80% of participating farmers have embraced our technology.</li>
      </ul>
    </div>

  <div id="stories" class="tab-content">
      <h2>Success Stories</h2>
      <p>Real stories of transformation from our community of farmers:</p>
      <ul>
        <li><strong>Siddharthnagar Triumph:</strong> "Thanks to AI insights, I doubled my yield despite erratic weather." – Ramesh.</li>
        <li><strong>Balrampur Breakthrough:</strong> "Smart irrigation recommendations saved my crops during a drought." – Sita.</li>
        <li><strong>Varanasi Victory:</strong> "Personalized crop planning turned my small plot into a thriving organic farm." – Arjun.</li>
      </ul>
    </div>

  <div id="resources" class="tab-content">
      <h2>Resources & Practical Tips</h2>
      <p>Stay updated with the latest resources to uplift your farming practices:</p>
      <ul>
        <li><strong>Guides & Tutorials:</strong> Step-by-step sustainable practices.</li>
        <li><strong>Best Practices:</strong> Learn from success stories and strategic interventions.</li>
        <li><strong>Partnerships:</strong> Connect with NGOs, experts, and government programs.</li>
      </ul>
    </div>
  </div>

  <div class="cta">
    <button onclick="showMoreInfo()">Learn More</button>
  </div>

  <div id="additional-info">
    <h3>Empowering Farmers with AI</h3>
    <p>Small and marginal farmers face challenges such as climate change, resource constraints, and unsustainable practices...</p>
  </div>

  <script>
      
  
  
  <!-- JavaScript for Form Handling & Animation -->
  <script>
  document.addEventListener('DOMContentLoaded', function () {
    const form = document.getElementById('contactForm');
    const successMessage = document.getElementById('successMessage');
  
    form.addEventListener('submit', function (e) {
      e.preventDefault(); // Prevent default form submission
      successMessage.style.display = 'block'; // Show success message
      successMessage.style.opacity = '0'; // Start with hidden opacity
      successMessage.style.transform = 'translateY(-20px)'; // Start with slide-up effect
  
      // Trigger animation
      setTimeout(() => {
        successMessage.style.transition = 'opacity 0.5s, transform 0.5s'; // Smooth transition
        successMessage.style.opacity = '1'; // Fade-in effect
        successMessage.style.transform = 'translateY(0)'; // Slide down into position
      }, 10);
  
      // Hide the success message after 3 seconds
      setTimeout(() => {
        successMessage.style.transition = 'opacity 0.5s'; // Smooth fade-out effect
        successMessage.style.opacity = '0';
        setTimeout(() => {
          successMessage.style.display = 'none'; // Completely hide the message
        }, 500); // Wait for the fade-out to complete
      }, 3000);
  
      form.reset(); // Reset the form fields
    });
  });
  </script>
  

<!-- Footer -->
<footer>
<p>© 2025 Empowering Farmers Initiative. All Rights Reserved.</p>
<p>
  <a href="privacy-policy.html">Privacy Policy</a> |
  <a href="chintu">chintu</a> 
  <a href="terms-of-service.html">Terms of Service</a>
</p>
<p>
  Connect with us: 
  <a href="#">Facebook</a> | 
  <a href="#">Twitter</a> | 
  <a href="#">LinkedIn</a>
</p>
</footer>

<!-- JavaScript for Tab Navigation & Form Handling -->
<script>
document.addEventListener('DOMContentLoaded', function() {
  // Tab switching logic
  const tabs = document.querySelectorAll('.tab-header li');
  const contents = document.querySelectorAll('.tab-content');
  
  tabs.forEach(tab => {
    tab.addEventListener('click', function() {
      const targetTab = this.getAttribute('data-tab');
      
      // Remove active class from all tabs and contents
      tabs.forEach(item => item.classList.remove('active'));
      contents.forEach(content => content.classList.remove('active'));
      
      // Activate the clicked tab and its corresponding content
      this.classList.add('active');
      document.getElementById(targetTab).classList.add('active');
    });
  });
  
  // Contact form submission demonstration
  document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Thank you for getting in touch! We will respond soon.');
    this.reset();
  });
});
</script>
</body>
</html>
