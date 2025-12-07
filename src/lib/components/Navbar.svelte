<script lang="ts">
  import { onMount } from 'svelte';

  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 0;
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<nav class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 {isScrolled ? 'bg-white/80 backdrop-blur-md border-b border-gray-100 py-3' : 'bg-transparent py-5'}">
  <div class="max-w-7xl mx-auto px-6 flex items-center justify-between">
    <div class="flex items-center gap-12">
      <a href="/" class="text-2xl font-bold tracking-tighter">V7</a>
      
      <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-600">
        <a href="#" class="hover:text-black transition-colors">Product</a>
        <a href="#" class="hover:text-black transition-colors">AI Agents</a>
        <a href="#" class="hover:text-black transition-colors">Pricing</a>
        <a href="#" class="hover:text-black transition-colors">Resources</a>
      </div>
    </div>

    <div class="flex items-center gap-4 text-sm font-medium">
      <a href="#" class="hidden md:block hover:text-gray-600 transition-colors">Log in</a>
      <a href="#" class="bg-black text-white px-4 py-2 rounded-full hover:bg-gray-800 transition-colors">Book a demo</a>
    </div>
  </div>
</nav>
