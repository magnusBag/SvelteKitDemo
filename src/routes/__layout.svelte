<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
</script>

<div class=" bg-black px-4 ">
  <div class="image">
    <Nav />
    <main>
      <slot />
    </main>
  </div>
</div>

<style>
  @media screen and (min-width: 480px) {
    .image {
      background-position: 50% 45%;
    }
  }
  .image {
    background: url("https://i.ibb.co/LpfJr5r/Farve.png");
    background-position: 50% 190px;
    background-repeat: no-repeat;
    background-size: 60vw;

    background-attachment: fixed;
    backdrop-filter: blur(4px);
  }
  main {
    font-family: "Poppins", sans-serif;
  }
</style>
