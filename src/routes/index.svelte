<script>
  import texts from "../lib/texts.json";
  import Contentgrid from "../components/contentgrid.svelte";
  import Maps from "../components/Maps.svelte";
  import Timer from "../components/Timer.svelte";
</script>

<svelte:head>
  <title>Kanten</title>
</svelte:head>

<div class="p-2">
  <!-- titel -->

  <div class="grid w-full mt-2 sm:-mt-4 mb-[30vh] ">
    <span class="block justify-self-center mb-9 mt-6 " />
    <div class="flex text-white w-full justify-evenly text-4xl uppercase ">
      <p>k</p>
      <p>a</p>
      <p>n</p>
      <p>t</p>
      <p>e</p>
      <p>n</p>
    </div>
    <Timer />
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

    <div id="textgrid" class="bg-black p-4 my-4  rounded-md lg:w-128 mx-auto  ">
      <h1 class="text-2xl my-5 uppercase text-white text-center px-2 ">
        <b>om kanten</b>
      </h1>
      <span class="block justify-self-center" />
      <p class="text-md my-5 text-white px-2">{texts.text2}</p>
    </div>
  </a>

  <!-- grid -->
  <Contentgrid {texts} />
  <!-- maps -->
  <Maps mapKanten={texts.mapkanten} mapKraftværket={texts.mapkraftværk} />
</div>

<style>
</style>
