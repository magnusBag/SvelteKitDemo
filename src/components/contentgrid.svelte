<script>
  export let texts;
</script>

<div
  class="grid grid-cols-1 bg-black lg:rounded-md place-items-center mb-4 gap-3 lg:grid-cols-2 lg:w-128 w-full mx-auto h-center"
>
  <div class="w-fill  h-full rounded-md bg-black ">
    <img
      class="my-5 lg:mt-28 rounded-md "
      src={"https://mbaggesen.com/lib/Billede1.png"}
      alt="Katenbillede1"
    />
    <h1 class="text-lg text-center pb-1 text-white">
      <b>{texts.titel1}</b>
    </h1>
    <div class="w-fill h-fill rounded-md bg-black ">
      <p class="text-md my-5 text-white ">{texts.text1}</p>
      <p class="text-lg my-3 text-white font-[600]">{texts.text4}.</p>
    </div>
  </div>
  <div class=" rounded-md bg-black ">
    <img
      class="my-5 rounded-md  "
      src={"https://mbaggesen.com/lib/Billede2.png"}
      alt="Katenbillede1"
    />
    <div class="flex rounded-md overflow-hidden max-h-[30vh]">
      <img
        src="https://mbaggesen.com/lib/Billede3.png"
        alt="Kanten studio"
        class="w-1/2"
      />
      <img
        src="https://mbaggesen.com/lib/billede4.png"
        alt="Kanten studio"
        class="w-1/2"
      />
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
