<script>
  import Header from './Header.svelte';
  import Footer from './Footer.svelte';
</script>

<Header />

<main id="home" class="bg-white text-slate-800">
  
  <!-- Hero Section -->
  <section class="relative h-[85vh] sm:h-screen">
    <video
      autoplay
      loop
      playsinline
      muted
      class="absolute inset-0 w-full h-full object-cover -z-0"
    >
      <source src="assets/out.mp4" type="video/mp4"/>
    </video>
    <div class="absolute inset-0 bg-black/60 z-10"></div>
    <div class="relative z-20 flex flex-col items-center justify-center h-full text-white px-4">
      <div class="py-8 flex flex-col items-center text-center max-w-3xl">
        <h1 class="text-3xl sm:text-5xl font-bold tracking-tight">
          Building excellence across industries
        </h1>
        <p class="mt-4 text-base sm:text-lg text-slate-200 max-w-xl leading-relaxed">
          Metse Henofa Holdings is your trusted partner in navigating complex business landscapes. From construction to financial security, we provide comprehensive solutions tailored to your needs.
        </p>
        <a 
          href="#contact" 
          class="mt-6 inline-flex items-center space-x-2 bg-orange-500 hover:bg-orange-600 text-white font-medium text-sm px-5 py-2.5 rounded-full transition duration-200 shadow-md focus:outline-none focus:ring-2 focus:ring-orange-400"
        >
          <span>Start your journey</span>
          <span>&rarr;</span>
        </a>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="py-16 px-4 sm:px-6 lg:px-8 bg-slate-50">
    <div class="max-w-7xl mx-auto">
      <div class="text-center max-w-2xl mx-auto mb-10">
        <h2 class="text-2xl sm:text-3xl font-bold text-slate-900 tracking-tight">
          Comprehensive Business Solutions
        </h2>
        <p class="mt-2 text-sm sm:text-base text-slate-600">
          Empowering growth and delivering excellence across a diverse range of industry sectors.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        
        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-person-digging text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Construction & Development
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            From infrastructure planning to project management, we build the foundations of your vision with precision and quality.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-scale-balanced text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Consulting & Compliance
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Navigate regulatory landscapes with confidence. Our experts ensure your business remains compliant while optimizing growth strategies.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-shield-halved text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Security Services
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Protect your assets and people with our state-of-the-art security solutions, ranging from physical guarding to surveillance systems.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-sack-dollar text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Micro Loans & Finance
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Access flexible financial solutions designed to support individuals and small businesses in achieving their economic goals.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-house-chimney text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Real Estate
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Find your perfect property or maximize your investment potential with our expert real estate advisory and management services.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-wrench text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Auto Mechanical
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Reliable vehicle maintenance and repair services ensuring your fleet or personal vehicle runs at peak performance.
          </p>
        </div>

        <div class="bg-white border border-slate-200/80 rounded-xl p-6 shadow-sm hover:shadow-md transition duration-200">
          <div class="w-12 h-12 rounded-full bg-amber-100 flex items-center justify-center mb-4">
            <i class="fa-solid fa-tower-cell text-amber-600 text-lg"></i>
          </div>
          <h3 class="text-lg font-serif font-bold text-slate-900 mb-2">
            Telecommunications
          </h3>
          <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
            Providing robust communication infrastructure and connectivity solutions to keep your business linked and productive.
          </p>
        </div>

      </div>
    </div>
  </section>

  <!-- About / Leadership Section -->
  <section id="about" class="py-16 px-4 sm:px-6 lg:px-8 bg-slate-100">
    <div class="max-w-7xl mx-auto">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-10 lg:gap-14 items-center">
        
        <div class="space-y-4">
          <div>
            <span class="text-orange-500 font-semibold tracking-wider uppercase text-xs">
              Leadership
            </span>
            <h2 class="text-2xl sm:text-3xl font-bold font-serif text-slate-900 mt-1">
              Visionary Leadership
            </h2>
            <p class="text-orange-600 font-medium text-base mt-1">
              Founder &amp; CEO: Mr Phineus Motlatso Mothabeng
            </p>
          </div>

          <p class="text-slate-600 text-sm leading-relaxed">
            At Metse Henofa Holdings, we believe that every challenge presents an opportunity for growth. Under the leadership of Mr. Mothabeng, our team is dedicated to providing practical, effective solutions for those in need of guidance.
          </p>

          <p class="text-slate-600 text-sm leading-relaxed">
            We don't just offer services; we build longer lasting relationships based on trust, integrity, and a genuine desire to see our clients succeed. Whether you are a corporation seeking compliance or an individual needing financial advice, we are here to help.
          </p>

          <div class="grid grid-cols-2 gap-4 pt-2 border-t border-slate-200">
            <div class="bg-white border border-slate-200 rounded-lg p-4 shadow-sm">
              <div class="flex items-center space-x-2 mb-1">
                <i class="fa-solid fa-award text-orange-500 text-lg"></i>
                <span class="text-2xl font-extrabold text-slate-900">10+</span>
              </div>
              <p class="text-slate-500 text-xs font-medium">Years Experience</p>
            </div>

            <div class="bg-white border border-slate-200 rounded-lg p-4 shadow-sm">
              <div class="flex items-center space-x-2 mb-1">
                <i class="fa-solid fa-layer-group text-orange-500 text-lg"></i>
                <span class="text-2xl font-extrabold text-slate-900">8</span>
              </div>
              <p class="text-slate-500 text-xs font-medium">Diverse Industries</p>
            </div>
          </div>
        </div>

        <div class="relative flex justify-center lg:justify-end">
          <div class="relative w-full max-w-md rounded-xl overflow-hidden shadow-xl border border-slate-200">
            <img 
              src="https://images.unsplash.com/photo-1560250097-0b93528c311a?auto=format&fit=crop&q=80&w=800" 
              alt="Mr Phineus Motlatso Mothabeng" 
              class="w-full h-[380px] sm:h-[450px] object-cover object-top"
            />
            <div class="absolute bottom-0 inset-x-0 bg-slate-900/85 backdrop-blur-md p-3 border-t border-white/10 text-white">
              <p class="font-semibold text-sm">Mr Phineus Motlatso Mothabeng</p>
              <p class="text-orange-400 text-xs">Founder &amp; CEO, Metse Henofa Holdings</p>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Our Work Section -->
  <section id="work" class="py-16 px-4 sm:px-6 lg:px-8 bg-slate-50">
    <div class="max-w-7xl mx-auto">
      
      <div class="text-center max-w-2xl mx-auto mb-10">
        <span class="text-orange-500 font-semibold tracking-wider uppercase text-xs">
          Our Expertise
        </span>
        <h2 class="text-2xl sm:text-3xl font-bold font-serif text-slate-900 mt-1">
          Projects &amp; Operations
        </h2>
        <p class="mt-2 text-sm sm:text-base text-slate-600">
          A glimpse into the diverse range of projects and professional environments we manage across South Africa.
        </p>
      </div>

      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
        
        <figure class="group relative rounded-xl overflow-hidden bg-slate-800 h-64 shadow-md">
          <img 
            src="https://images.unsplash.com/photo-1541888946425-d0fbb186a5b3?auto=format&fit=crop&q=80&w=600" 
            alt="Infrastructure Development" 
            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
          />
          <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/30 to-transparent opacity-80"></div>
          <figcaption class="absolute bottom-0 inset-x-0 p-4">
            <span class="text-orange-400 text-[10px] font-semibold uppercase tracking-wider">Sector</span>
            <h3 class="text-base font-bold text-white">Infrastructure Development</h3>
          </figcaption>
        </figure>

        <figure class="group relative rounded-xl overflow-hidden bg-slate-800 h-64 shadow-md">
          <img 
            src="https://images.unsplash.com/photo-1557804506-669a67965ba0?auto=format&fit=crop&q=80&w=600" 
            alt="Professional Security" 
            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
          />
          <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/30 to-transparent opacity-80"></div>
          <figcaption class="absolute bottom-0 inset-x-0 p-4">
            <span class="text-orange-400 text-[10px] font-semibold uppercase tracking-wider">Sector</span>
            <h3 class="text-base font-bold text-white">Professional Security</h3>
          </figcaption>
        </figure>

        <figure class="group relative rounded-xl overflow-hidden bg-slate-800 h-64 shadow-md">
          <img 
            src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&q=80&w=600" 
            alt="Facility Management" 
            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
          />
          <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/30 to-transparent opacity-80"></div>
          <figcaption class="absolute bottom-0 inset-x-0 p-4">
            <span class="text-orange-400 text-[10px] font-semibold uppercase tracking-wider">Sector</span>
            <h3 class="text-base font-bold text-white">Facility Management</h3>
          </figcaption>
        </figure>

        <figure class="group relative rounded-xl overflow-hidden bg-slate-800 h-64 shadow-md">
          <img 
            src="https://images.unsplash.com/photo-1486006920555-c77dce18193b?auto=format&fit=crop&q=80&w=600" 
            alt="Auto Mechanical Services" 
            class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
          />
          <div class="absolute inset-0 bg-gradient-to-t from-slate-950 via-slate-950/30 to-transparent opacity-80"></div>
          <figcaption class="absolute bottom-0 inset-x-0 p-4">
            <span class="text-orange-400 text-[10px] font-semibold uppercase tracking-wider">Sector</span>
            <h3 class="text-base font-bold text-white">Auto Mechanical Services</h3>
          </figcaption>
        </figure>

      </div>
    </div>
  </section>

</main>
