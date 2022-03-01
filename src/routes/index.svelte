<script>
  import texts from "../lib/texts.json";
  import Contentgrid from "../components/contentgrid.svelte";
  import Maps from "../components/Maps.svelte";
</script>

<svelte:head>
  <title>Welcome page</title>
</svelte:head>

<div class="p-2">
  <!-- titel -->
  <div class="grid w-full mt-8 sm:mt-2 ">
    <span class="block justify-self-center mb-9 mt-6 " />
    <h1
      class="text-3xl sm:text-4xl tracking-[0.4em] text-center my-2 mb-40 sm:mb-80 uppercase text-white"
    >
      K a n t e n
    </h1>
  </div>
  <!-- om os tekst -->
  <div class="bg-black p-4 my-6 lg:mt-96 rounded-md lg:w-128 mx-auto  ">
    <h1 class="text-2xl my-5 uppercase text-white text-center px-2 ">
      <b>om kanten</b>
    </h1>
    <span class="block justify-self-center" />
    <p class="text-md my-5 text-white px-2">{texts.text2}</p>
  </div>

  <!-- grid -->
  <Contentgrid {texts} />
  <!-- maps -->
  <Maps mapKanten={texts.mapkanten} mapKraftværket={texts.mapkraftværk} />
</div>

<style>
</style>
