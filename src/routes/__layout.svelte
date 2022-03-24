<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
  import Footer from "../components/footer.svelte";
</script>

<div class="bg-black px-4 ">
  <Nav />
  <main>
    <slot />
  </main>
  <Footer />
</div>

<style>
  main {
    font-family: "Poppins", sans-serif;
  }
</style>
