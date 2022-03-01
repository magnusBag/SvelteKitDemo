<script>
  export let texts;
</script>

<div
  class="grid grid-cols-1 lg:bg-black lg:rounded-md  place-items-center gap-3 lg:grid-cols-2 lg:w-128 w-full mx-auto"
>
  <div class="w-fill px-2 h-full rounded-md bg-black ">
    <img
      class="my-5 rounded-md px-2"
      src={"https://usercontent.one/wp/www.kanten-esbjerg.dk/wp-content/uploads/2022/02/IMG_0753-1024x768.png"}
      alt="Katenbillede1"
    />
    <h1 class="text-lg text-center pb-1 text-white">
      <b>{texts.titel1}</b>
    </h1>
    <div class="w-fill h-fill rounded-md bg-black px-2">
      <p class="text-md my-5 text-white ">{texts.text1}</p>
    </div>
  </div>
  <div class="w-fill rounded-md px-2  bg-black ">
    <img
      class="my-5 rounded-md px-2 "
      src={"https://usercontent.one/wp/www.kanten-esbjerg.dk/wp-content/uploads/2022/02/IMG_0363-1024x768.png"}
      alt="Katenbillede1"
    />
    <h1 class="text-lg text-center pb-1 text-white">
      <b>{texts.titel3}</b>
    </h1>
    <div class="w-fill rounded-md bg-black px-2">
      <p class="text-md my-5 text-white ">{texts.text3}</p>
    </div>
  </div>
</div>
