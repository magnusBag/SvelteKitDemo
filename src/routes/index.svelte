<script>
  import ImagePost from "../components/imagePost.svelte";
  import { text1, text2 } from "../../static/texts.json";
</script>

<svelte:head>
  <title>Welcome page</title>
</svelte:head>

<h1 class="text-4xl text-center my-5 uppercase text-white">K a n t e n</h1>

<h1 class="text-2xl text-center my-5 uppercase text-white  bg-black p-6">
  om kanten
</h1>

<div class="grid grid-cols-1 gap-3 content-center sm:grid-cols-2 sm:px-24 ">
  <div class="w-fill rounded-sm  bg-black p-3">
    <p class="text-sm text-left my-5 text-white ">{text2}</p>
  </div>
  <ImagePost src={"../../static/Billede1.png"} />
  <div class="w-fill rounded-sm bg-black p-5">
    <p class="text-sm text-left my-5 text-white ">{text1}</p>
  </div>
  <div class="w-fill rounded-sm bg-black p-5">
    <iframe
      title="kantenmap"
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d36182.88061459491!2d8.461398805123324!3d55.472602203794416!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x464b212b863b9f21%3A0xda996a903b7c0df7!2sFinsensgade%201%2C%206700%20Esbjerg!5e0!3m2!1sen!2sdk!4v1645955380398!5m2!1sen!2sdk"
      width="100%"
      height="100%"
      style="border:0;"
      allowfullscreen=""
      loading="lazy"
    />
  </div>
</div>
