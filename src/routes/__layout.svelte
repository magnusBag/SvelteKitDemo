<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
  import Footer from "../components/footer.svelte";
</script>

<div class="bg-black px-4 ">
  <div class="image">
    <Nav />
    <main>
      <slot />
    </main>
    <Footer />
  </div>
</div>

<style>
  .image {
    background-image: url("https://i.ibb.co/LpfJr5r/Farve.png");
    background-position: 50% 190px;
    background-repeat: no-repeat;
    background-size: 55vw;
    background-attachment: fixed;
  }
  @media (max-width: 450px) {
    .image {
      background-size: 80vw;
    }
  }
  @media (min-width: 1020px) {
    .image {
      background-size: 75vw;
    }
  }
  @media (min-width: 1400px) {
    .image {
      background-size: 55vw;
    }
  }
  main {
    font-family: "Poppins", sans-serif;
  }
  html {
    scroll-behavior: smooth;
  }
</style>
