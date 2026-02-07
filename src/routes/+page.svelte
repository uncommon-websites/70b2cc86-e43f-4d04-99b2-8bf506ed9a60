<script>
  import Header from "$lib/Header.svelte";
  import Hero from "$lib/Hero.svelte";
  import Logos from "$lib/Logos.svelte";
  import WhyPolymarket from "$lib/WhyPolymarket.svelte";
  import Products from "$lib/Products.svelte";
  import FoundersBanner from "$lib/FoundersBanner.svelte";
  import FAQ from "$lib/FAQ.svelte";
  import FooterCTA from "$lib/FooterCTA.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<div class="min-h-screen bg-white font-sans selection:bg-primary-500 selection:text-white text-gray-900">
  <Header />
  
  <main>
    <Hero />
    <Logos />
    <WhyPolymarket />
    <Products />
    <FoundersBanner />
    <FAQ />
    <FooterCTA />
  </main>

  <Footer />
</div>

