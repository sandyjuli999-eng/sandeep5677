
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>eSmart Home Tuition</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"/>
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>

  <script type="text/javascript">
    (function(){ emailjs.init("Sandeep parajuli"); })();
    document.addEventListener('DOMContentLoaded', function() { AOS.init({duration:1000, once:true}); });
  </script>

  <style>
    body { scroll-behavior: smooth; }
    .hero-background {
      background-image: url('https://images.unsplash.com/photo-1596496052176-94f0184fae69?auto=format&fit=crop&w=1600&q=80');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      animation: zoomIn 20s infinite alternate;
    }
    .hero-overlay { background: rgba(0, 0, 0, 0.5); }
    @keyframes zoomIn { from { transform: scale(1); } to { transform: scale(1.05); } }
    .card-hover:hover { transform: scale(1.05); box-shadow: 0 10px 25px rgba(0,0,0,0.2); transition: all 0.3s ease; }
    .button-hover:hover { background-position: right center; transition: all 0.4s ease; }
    .screenshot { margin-top: 10px; max-width: 100%; border: 1px solid #ccc; border-radius: 8px; transition: transform 0.3s ease; display: block; }
    .screenshot:hover { transform: scale(1.1); }
  </style>
</head>
<body class="bg-gray-50 text-gray-800">

<!-- Navbar -->
<nav class="bg-gradient-to-r from-blue-500 to-purple-600 shadow-lg fixed w-full z-10">
  <div class="max-w-7xl mx-auto px-4 py-3 flex justify-between items-center">
    <h1 class="text-2xl italic font-bold text-white">eSmart Home Tuition</h1>
    <a href="#register" class="bg-white text-blue-600 px-4 py-2 rounded-lg hover:bg-gray-100 transition">Register</a>
  </div>
</nav>

<!-- Hero Section -->
<section class="h-screen relative hero-background">
  <div class="absolute inset-0 hero-overlay flex items-center justify-center">
    <div class="text-center px-4 text-white" data-aos="fade-up">
      <h2 class="text-4xl md:text-5xl font-bold italic">_eSmart Home Tuition_</h2>
      <p class="mt-4 text-lg md:text-xl">Personalized Online Tuition with Flexible Scheduling</p>
      <p class="mt-2 text-md">Subjects: Math & Science (Chemistry)</p>
      <a href="#register" class="mt-6 inline-block bg-gradient-to-r from-blue-500 to-purple-500 px-6 py-3 rounded-lg font-semibold shadow-lg button-hover">Book a Slot</a>
    </div>
  </div>
</section>

<!-- Subjects Section -->
<section id="subjects" class="py-16 bg-gray-100">
  <div class="max-w-5xl mx-auto px-6 text-center">
    <h3 class="text-3xl font-semibold text-blue-700 mb-8" data-aos="fade-up">Subjects Offered</h3>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="p-6 bg-white rounded-2xl shadow card-hover" data-aos="fade-right">
        <i class="fas fa-square-root-alt text-4xl text-blue-500"></i>
        <h4 class="mt-4 text-xl font-semibold">Mathematics</h4>
        <p class="mt-2 text-gray-600">Step-by-step explanations, problem-solving, and exam preparation.</p>
      </div>
      <div class="p-6 bg-white rounded-2xl shadow card-hover" data-aos="fade-left">
        <i class="fas fa-flask text-4xl text-purple-500"></i>
        <h4 class="mt-4 text-xl font-semibold">Science (Chemistry)</h4>
        <p class="mt-2 text-gray-600">Clear concepts, practical applications, and strong fundamentals.</p>
      </div>
    </div>
  </div>
</section>

<!-- Schedule Section -->
<section id="schedule" class="py-16 bg-white">
  <div class="max-w-3xl mx-auto text-center px-6">
    <h3 class="text-3xl font-semibold text-blue-700 mb-8" data-aos="fade-up">Available Time Slots</h3>
    <div class="grid md:grid-cols-2 gap-6">
      <div class="p-6 bg-gradient-to-r from-blue-400 to-purple-400 text-white rounded-2xl shadow card-hover" data-aos="fade-right">
        <i class="fas fa-sun text-3xl"></i>
        <h4 class="mt-2 text-xl font-semibold">Morning</h4>
        <p>7:00 AM – 8:00 AM</p>
      </div>
      <div class="p-6 bg-gradient-to-r from-purple-400 to-blue-400 text-white rounded-2xl shadow card-hover" data-aos="fade-left">
        <i class="fas fa-moon text-3xl"></i>
        <h4 class="mt-2 text-xl font-semibold">Evening</h4>
        <p>5:00 PM – 6:00 PM</p>
      </div>
    </div>
  </div>
</section>

<!-- Registration Section -->
<section id="register" class="py-16 bg-gray-50">
  <div class="max-w-3xl mx-auto px-6">
    <h3 class="text-3xl font-semibold text-center text-blue-700 mb-8" data-aos="fade-up">Register for Tuition</h3>
    <form id="tuitionForm" class="space-y-6 bg-white p-6 rounded-2xl shadow-lg" data-aos="fade-up" enctype="multipart/form-data">
      <div>
        <label class="block mb-2 font-medium">Full Name</label>
        <input name="name" type="text" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400" required>
      </div>
      <div>
        <label class="block mb-2 font-medium">Email</label>
        <input name="email" type="email" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400" required>
      </div>
      <div>
        <label class="block mb-2 font-medium">Phone Number</label>
        <input name="phone" type="tel" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400" required>
      </div>
      <div>
        <label class="block mb-2 font-medium">Preferred Time Slot</label>
        <select name="timeslot" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400" required>
          <option value="">Select a time</option>
          <option>Morning (7–8 AM)</option>
          <option>Evening (5–6 PM)</option>
        </select>
      </div>
      <div>
        <label class="block mb-2 font-medium">Subject</label>
        <select name="subject" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400" required>
          <option value="">Select subject</option>
          <option>Math</option>
          <option>Science (Chemistry)</option>
        </select>
      </div>
      <div class="bg-gray-100 p-4 rounded-lg border">
        <p class="font-semibold mb-2">Advance Payment via eSewa</p>
        <p class="mb-2">Pay to eSewa Number: <span class="font-bold">9869935664</span></p>
        <label class="block mb-2 font-medium">Transaction ID</label>
        <input name="transaction" type="text" placeholder="Enter eSewa Transaction ID" class="w-full px-4 py-2 rounded-lg border focus:ring-2 focus:ring-blue-400">
        <label class="block mt-4 mb-2 font-medium">Upload Payment Screenshot</label>
        <input name="screenshot" type="file" accept="image/*" class="w-full">
      </div>
      <button type="submit" class="w-full bg-gradient-to-r from-blue-500 to-purple-500 text-white px-6 py-3 rounded-lg font-semibold shadow-lg hover:from-purple-500 hover:to-blue-500 transition">Submit Registration</button>
    </form>

    <!-- Confirmation Message with Pay Now Button -->
    <div id="confirmationMessage" class="hidden mt-6 p-6 bg-green-100 rounded-lg text-center text-green-800 font-semibold">
      ✅ Registration Successful! Please complete your payment below:
      <br>
      <a href="https://esewa.com.np/#/home?recipient=9869935664" target="_blank" 
         class="inline-block mt-4 px-6 py-3 bg-gradient-to-r from-blue-500 to-purple-500 text-white rounded-lg font-semibold hover:from-purple-500 hover:to-blue-500 transition">
         💰 Pay Now via eSewa
      </a>
    </div>
  </div>
</section>

<!-- Contact Section -->
<section id="contact" class="py-12 bg-white" data-aos="fade-up">
  <div class="max-w-3xl mx-auto text-center px-6">
    <h3 class="text-2xl font-semibold text-blue-700 mb-4">Contact Us</h3>
    <p class="text-gray-700">For inquiries, call us at <span class="font-bold">9869935664</span> or email: <span class="font-bold">sandyjuli999@gmail.com</span></p>
  </div>
</section>

<!-- Footer -->
<footer class="bg-gradient-to-r from-blue-500 to-purple-600 text-white text-center py-4">
  <p>&copy; 2025 eSmart Home Tuition. All rights reserved.</p>
</footer>

<!-- Scripts -->
<script>
  document.getElementById('tuitionForm').addEventListener('submit', function(event){
    event.preventDefault();
    const form = this;
    const screenshotInput = form.querySelector('input[name="screenshot"]');
    
    if(screenshotInput.files.length > 0){
      const file = screenshotInput.files[0];
      const reader = new FileReader();
      reader.onload = function() {
        let base64Field = form.querySelector('input[name="screenshot_base64"]');
        if(!base64Field){
          base64Field = document.createElement('input');
          base64Field.type = 'hidden';
          base64Field.name = 'screenshot_base64';
          form.appendChild(base64Field);
        }
        base64Field.value = reader.result;
        sendEmailJSForm(form);
      }
      reader.readAsDataURL(file);
    } else {
      sendEmailJSForm(form);
    }
  });

  function sendEmailJSForm(form){
    emailjs.sendForm('service_k85uamt', 'template_xapof57', form)
      .then(() => {
        form.classList.add('hidden'); // hide form
        document.getElementById('confirmationMessage').classList.remove('hidden'); // show confirmation
        document.getElementById('confirmationMessage').scrollIntoView({ behavior: 'smooth' });
      }, (error) => {
        alert('Oops! Something went wrong. ' + JSON.stringify(error));
      });
  }
</script>

<script>
  AOS.init({duration:1000, once:true});
</script>
</body>
</html>
