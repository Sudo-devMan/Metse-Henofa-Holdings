<script>
  let isOpen = $state(false);

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<header class="sticky top-0 z-50 backdrop-blur-md bg-white/80 border-b border-slate-200 shadow-sm transition-colors duration-300">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex items-center justify-between h-16">
      
      <!-- Brand Title -->
      <a href="#home" class="text-lg sm:text-xl font-bold tracking-tight text-slate-900 hover:text-orange-500 transition duration-200">
        Metse Henofa Holdings
      </a>

      <!-- Desktop Navigation -->
      <nav class="hidden md:flex items-center space-x-6 text-sm font-medium text-slate-700">
        <a href="#home" class="hover:text-orange-500 transition duration-200">Home</a>
        <a href="#services" class="hover:text-orange-500 transition duration-200">Services</a>
        <a href="#about" class="hover:text-orange-500 transition duration-200">About</a>
        <a href="#work" class="hover:text-orange-500 transition duration-200">Our Work</a>
        <a href="#contact" class="hover:text-orange-500 transition duration-200">Contact</a>
      </nav>

      <!-- Desktop Controls -->
      <div class="hidden md:flex items-center space-x-4">
        <!-- CTA Button -->
        <a href="#contact" class="bg-orange-500 hover:bg-orange-600 text-white font-semibold text-sm px-4 py-2 rounded-full transition duration-200 shadow-sm">
          Get Quote
        </a>
      </div>

      <!-- Mobile Right Items -->
      <div class="md:hidden flex items-center space-x-2">
        <button onclick={toggleMenu} type="button" class="text-slate-700 p-2" aria-label="Toggle Menu">
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>

    </div>
  </div>

  <!-- Mobile Dropdown Menu -->
  {#if isOpen}
    <div class="md:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-6 space-y-3 text-center text-sm">
      <a href="#home" onclick={toggleMenu} class="block py-2 text-slate-700 hover:text-orange-500 font-medium">Home</a>
      <a href="#services" onclick={toggleMenu} class="block py-2 text-slate-700 hover:text-orange-500 font-medium">Services</a>
      <a href="#about" onclick={toggleMenu} class="block py-2 text-slate-700 hover:text-orange-500 font-medium">About</a>
      <a href="#work" onclick={toggleMenu} class="block py-2 text-slate-700 hover:text-orange-500 font-medium">Our Work</a>
      <a href="#contact" onclick={toggleMenu} class="block py-2 text-slate-700 hover:text-orange-500 font-medium">Contact</a>
      <div class="pt-2">
        <a href="#contact" onclick={toggleMenu} class="inline-block bg-orange-500 hover:bg-orange-600 text-white font-semibold px-5 py-2 rounded-full transition duration-200 shadow-sm">
          Get Quote
        </a>
      </div>
    </div>
  {/if}
</header>