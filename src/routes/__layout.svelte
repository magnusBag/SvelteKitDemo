<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
</script>

<div class=" bg-black px-4">
  <div class="image">
    <Nav />
    <main>
      <slot />
    </main>
  </div>
</div>

<style>
  .image {
    background: url("../static/Farve.png");
    background-position: top;
    background-repeat: repeat-y;
    background-size: 450px;
    background-attachment: fixed;
    backdrop-filter: blur(4px);
  }
  main {
    font-family: "Poppins", sans-serif;
  }
</style>
