<script>
  let name = $state('');
  let email = $state('');
  let message = $state('');

  function handleMailtoSubmit(event) {
    event.preventDefault();
    const subject = encodeURIComponent(`Enquiry from ${name}`);
    const body = encodeURIComponent(`Name: ${name}\nEmail: ${email}\n\nMessage:\n${message}`);
    window.location.href = `mailto:info@metsehenofaholdings.co.za?subject=${subject}&body=${body}`;
  }
</script>

<footer id="contact" class="bg-slate-900 text-white relative pt-14 pb-8 px-4 sm:px-6 lg:px-8 border-t border-slate-800">
  <div class="max-w-7xl mx-auto space-y-12">
    
    <!-- Top Contact & Form Section -->
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-10 items-start">
      
      <!-- Contact Info Header & Details -->
      <div class="space-y-4">
        <div>
          <span class="text-orange-500 font-semibold tracking-wider uppercase text-xs">
            Get In Touch
          </span>
          <h2 class="text-2xl sm:text-3xl font-bold font-serif text-white mt-1">
            Let's Solve Your Problem
          </h2>
        </div>

        <p class="text-slate-300 text-sm leading-relaxed max-w-lg">
          Ready to move forward? Contact us today for a consultation or quote. We are here to assist you in Johannesburg and beyond.
        </p>

        <!-- Direct Contact List -->
        <div class="space-y-3 pt-2">
          <a href="tel:+27820624348" class="flex items-center space-x-3 text-slate-300 hover:text-orange-400 transition duration-200">
            <div class="w-10 h-10 rounded-full bg-orange-500/10 border border-orange-500/20 flex items-center justify-center text-orange-500">
              <i class="fa-solid fa-phone text-sm"></i>
            </div>
            <span class="text-sm font-medium">+27 82 062 4348</span>
          </a>

          <a href="mailto:info@metsehenofaholdings.co.za" class="flex items-center space-x-3 text-slate-300 hover:text-orange-400 transition duration-200">
            <div class="w-10 h-10 rounded-full bg-orange-500/10 border border-orange-500/20 flex items-center justify-center text-orange-500">
              <i class="fa-solid fa-envelope text-sm"></i>
            </div>
            <span class="text-sm font-medium">info@metsehenofaholdings.co.za</span>
          </a>

          <div class="flex items-center space-x-3 text-slate-300">
            <div class="w-10 h-10 rounded-full bg-orange-500/10 border border-orange-500/20 flex items-center justify-center text-orange-500">
              <i class="fa-solid fa-location-dot text-sm"></i>
            </div>
            <span class="text-sm font-medium">Johannesburg, South Africa</span>
          </div>
        </div>
      </div>

      <!-- Contact Form -->
      <div class="bg-slate-800/80 border border-slate-700/60 rounded-xl p-6 shadow-lg">
        <form onsubmit={handleMailtoSubmit} class="space-y-4">
          <div>
            <label for="name" class="block text-xs font-medium text-slate-300 mb-1">Name</label>
            <input 
              bind:value={name}
              type="text" 
              id="name" 
              required
              placeholder="Your Name" 
              class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3.5 py-2 text-sm text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-orange-500 focus:border-transparent transition duration-200"
            />
          </div>

          <div>
            <label for="email" class="block text-xs font-medium text-slate-300 mb-1">Email</label>
            <input 
              bind:value={email}
              type="email" 
              id="email" 
              required
              placeholder="your@email.com" 
              class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3.5 py-2 text-sm text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-orange-500 focus:border-transparent transition duration-200"
            />
          </div>

          <div>
            <label for="message" class="block text-xs font-medium text-slate-300 mb-1">Message</label>
            <textarea 
              bind:value={message}
              id="message" 
              rows="3" 
              required
              placeholder="How can we help you?" 
              class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3.5 py-2 text-sm text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-orange-500 focus:border-transparent transition duration-200 resize-none"
            ></textarea>
          </div>

          <button 
            type="submit" 
            class="w-full bg-orange-500 hover:bg-orange-600 text-white font-semibold py-2.5 px-5 text-sm rounded-lg transition duration-200 shadow hover:shadow-orange-500/25 focus:outline-none focus:ring-2 focus:ring-orange-400"
          >
            Send Enquiry
          </button>
        </form>
      </div>

    </div>

    <hr class="border-slate-800" />

    <!-- Bottom Links Grid -->
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
      
      <div class="space-y-2">
        <h3 class="text-base font-bold font-serif text-white tracking-wide">Metse Henofa</h3>
        <p class="text-slate-400 text-xs leading-relaxed">
          Your partner in comprehensive business solutions. Solving problems, building futures.
        </p>
      </div>

      <div>
        <h4 class="text-xs font-semibold text-white uppercase tracking-wider mb-3">Quick Links</h4>
        <ul class="space-y-2 text-xs text-slate-400">
          <li><a href="#home" class="hover:text-orange-400 transition duration-200">Home</a></li>
          <li><a href="#services" class="hover:text-orange-400 transition duration-200">Services</a></li>
          <li><a href="#about" class="hover:text-orange-400 transition duration-200">About Us</a></li>
          <li><a href="#contact" class="hover:text-orange-400 transition duration-200">Contact</a></li>
        </ul>
      </div>

      <div>
        <h4 class="text-xs font-semibold text-white uppercase tracking-wider mb-3">Services</h4>
        <ul class="space-y-2 text-xs text-slate-400">
          <li><a href="#services" class="hover:text-orange-400 transition duration-200">Construction</a></li>
          <li><a href="#services" class="hover:text-orange-400 transition duration-200">Consulting</a></li>
          <li><a href="#services" class="hover:text-orange-400 transition duration-200">Security</a></li>
          <li><a href="#services" class="hover:text-orange-400 transition duration-200">Finance</a></li>
        </ul>
      </div>

      <div>
        <h4 class="text-xs font-semibold text-white uppercase tracking-wider mb-3">Contact Info</h4>
        <ul class="space-y-2 text-xs text-slate-400">
          <li class="flex items-center space-x-2">
            <i class="fa-solid fa-location-dot text-orange-500"></i>
            <span>Johannesburg, South Africa</span>
          </li>
          <li class="flex items-center space-x-2">
            <i class="fa-solid fa-phone text-orange-500"></i>
            <a href="tel:+27820624348" class="hover:text-orange-400 transition duration-200">+27 82 062 4348</a>
          </li>
          <li class="flex items-center space-x-2">
            <i class="fa-solid fa-envelope text-orange-500"></i>
            <a href="mailto:info@metseenofaholdings.co.za" class="hover:text-orange-400 transition duration-200 break-all">info@metseenofaholdings.co.za</a>
          </li>
        </ul>
      </div>

    </div>

    <div class="pt-6 border-t border-slate-900 text-center text-xs text-slate-500">
      &copy; 2026 Metse Henofa Holdings (Pty) Ltd. All rights reserved.
    </div>

  </div>
</footer>