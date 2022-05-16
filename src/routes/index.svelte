<script context="module">
  export const prerender = true;
</script>

<script>
  import texts from "../lib/texts.json";
  import Contentgrid from "../components/contentgrid.svelte";
  import Maps from "../components/Maps.svelte";
</script>

<svelte:head>
  <title>KANTEN - Spillested</title>
</svelte:head>

<div class="p-2" id="welcome">
  <!-- titel -->

  <div
    class="grid grid-cols-1 place-items-center mt-2 sm:-mt-4  overflow-hidden mb-[50vh] lg:mb-[62vh] text-white"
  >
    <span class="block justify-self-center mb-9 mt-6" />
    <div class="flex w-full justify-evenly text-5xl uppercase ">
      <p>k</p>
      <p>a</p>
      <p>n</p>
      <p>t</p>
      <p>e</p>
      <p>n</p>
    </div>
    <p class="lg:text-[2vw] text-[4vw] mt-6 text-center">
      Esbjergs nye kulturfælleskab
    </p>
  </div>

  <!-- om os tekst -->
  <a href="#textgrid">
    <div
      class="grid grid-cols-1 place-items-center w-full mx-auto animate-bounce transition ease-in-out"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon icon-tabler icon-tabler-arrow-down"
        width="56"
        height="56"
        viewBox="0 0 24 24"
        stroke-width="3"
        stroke="#ffffff"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <line x1="18" y1="13" x2="12" y2="19" />
        <line x1="6" y1="13" x2="12" y2="19" />
      </svg>
    </div>

    <div
      id="textgrid"
      class="bg-black bg-opacity-40 my-4 py-2 rounded-md lg:w-128 mx-auto  "
    >
      <h1 class="text-2xl my-5 uppercase text-white text-center  ">
        <b>om kanten</b>
      </h1>
      <span class="block justify-self-center" />
      <p class="text-md my-5 text-white ">{texts.text2}</p>
    </div>
  </a>

  <!-- grid -->
  <Contentgrid {texts} />
  <!-- maps -->
  <Maps mapKanten={texts.mapkanten} mapKraftværket={texts.mapkraftværk} />
</div>
