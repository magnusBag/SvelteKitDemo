<script>
  import img1 from "../lib/Billede1.png";
  import img2 from "../lib/Billede2.png";
  import img3 from "../lib/Billede3.png";
  import img4 from "../lib/Billede4.png";

  export let texts;
</script>

<div
  class="grid grid-cols-1 bg-black lg:rounded-md place-items-center mb-4 gap-3 lg:grid-cols-2 lg:w-128 w-full mx-auto h-center"
>
  <div class="w-fill  h-full rounded-md bg-black ">
    <img class="my-5 lg:mt-28 rounded-md " src={img1} alt="Katenbillede1" />
    <h1 class="text-lg text-center pb-1 text-white">
      <b>{texts.titel1}</b>
    </h1>
    <div class="w-fill h-fill rounded-md bg-black ">
      <p class="text-md my-5 text-white ">{texts.text1}</p>
      <p class="text-lg my-3 text-white font-[600]">{texts.text4}.</p>
    </div>
  </div>
  <div class=" rounded-md bg-black ">
    <img class="my-5 rounded-md  " src={img2} alt="Katenbillede1" />
    <div class="flex rounded-md overflow-hidden max-h-[30vh]">
      <img src={img3} alt="Kanten studio" class="w-1/2" />
      <img src={img4} alt="Kanten studio" class="w-1/2" />
    </div>
    <h1 class="text-lg text-center py-2 text-white">
      <b>{texts.titel3}</b>
    </h1>
    <div class="w-fill rounded-md bg-black ">
      <p class="text-md my-5 text-white ">{texts.text3}</p>
    </div>
  </div>
  <div>
    <p class="text-white text-center text-4xl font-bold">Mere info følger.</p>
  </div>
</div>

<style>
  .h-center {
    align-content: center;
  }
</style>
