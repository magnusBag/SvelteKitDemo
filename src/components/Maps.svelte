<script>
  export let mapKraftværket;
  export let mapKanten;
</script>

<div
  grid
  class="grid grid-cols-1 md:grid-cols-2 gap-3 w-fill mx-auto lg:w-128 rounded-sm"
>
  <div>
    <h1 class="text-2xl text-white text-start"><b>KANTEN</b></h1>
    <span class="block mb-3" style="width: 9rem;" />
    <iframe
      width="100%"
      class="rounded-sm"
      src={mapKanten}
      title="kantenmap"
      style="border:0;"
      allowfullscreen=""
      loading="lazy"
    />
  </div>
  <div>
    <h1 class="text-2xl text-white text-start"><b>KRAFTVÆRKET</b></h1>
    <span class="block mb-3" style="width: 9rem;" />
    <iframe
      width="100%"
      class="rounded-sm"
      src={mapKraftværket}
      title="kantenmap"
      style="border:0;"
      allowfullscreen=""
      loading="lazy"
    />
  </div>
</div>
