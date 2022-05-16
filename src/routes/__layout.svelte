<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
  import Footer from "../components/footer.svelte";
</script>

<div class="bg-black overflow-hidden">
  <Nav />
  <div class="image">
    <main>
      <slot />
    </main>
  </div>
  <Footer />
</div>

<style>
  main {
    font-family: "Poppins", sans-serif;
    overflow: hidden;
    width: 100%;
  }
  .image {
    background-image: url("../lib/farve.png");
    background-position: 50% 250px;
    background-repeat: no-repeat;
    background-size: 55vw;
    background-attachment: fixed;
  }
  @media (max-width: 450px) {
    .image {
      background-size: 90vw;
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
  @media (min-width: 1900px) {
    .image {
      background-size: 40vw;
    }
  }
</style>
