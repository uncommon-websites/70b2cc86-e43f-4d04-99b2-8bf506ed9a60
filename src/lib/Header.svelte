<script>
  // Header component
</script>

<header class="flex items-center justify-between px-6 py-4 sticky top-0 bg-white/80 backdrop-blur-md z-50 border-b border-gray-100">
  <div class="flex items-center gap-2">
    <div class="font-bold text-xl tracking-tighter flex items-center gap-1.5 text-primary-600">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-600">
        <path d="M12 2L2 7L12 12L22 7L12 2Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M2 17L12 22L22 17" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M2 12L12 17L22 12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
      <span class="text-gray-900">Polymarket</span>
    </div>
  </div>

  <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-600">
    <a href="/" class="hover:text-primary-600 transition-colors">Markets</a>
    <a href="/" class="hover:text-primary-600 transition-colors">Activity</a>
    <a href="/" class="hover:text-primary-600 transition-colors">Leaderboard</a>
    <a href="/" class="hover:text-primary-600 transition-colors">Learn</a>
  </nav>

  <div class="flex items-center gap-4 text-sm">
    <a href="/" class="text-gray-600 font-medium hover:text-primary-600 transition-colors">Log in</a>
    <a href="/" class="bg-primary-600 text-white px-5 py-2.5 rounded-full font-medium hover:bg-primary-700 transition-all shadow-sm">Start Trading</a>
  </div>
</header>
