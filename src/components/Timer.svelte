<script>
  import { timerDone } from "../timerStore.js";
  var countDownDate = new Date("May 12 , 2022 18:00:00").getTime();
  let timerText = "__:__:__:__";
  var x = setInterval(function () {
    var now = new Date().getTime();
    var distance = countDownDate - now;
    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor(
      (distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)
    );
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);

    let secondsZero = "";
    if (seconds < 10) secondsZero = "0";

    let minutesZero = "";
    if (minutes < 10) minutesZero = "0";

    let hoursZero = "";
    if (hours < 10) hoursZero = "0";

    let daysZero = "";
    if (days < 10) daysZero = "0";

    timerText =
      daysZero +
      days +
      ":" +
      hoursZero +
      hours +
      ":" +
      minutesZero +
      minutes +
      ":" +
      secondsZero +
      seconds +
      "";

    if (distance < 0) {
      clearInterval(x);
      timerDone.set(true);
    }
  }, 1000);
</script>

<div class="mx-auto overflow-hidden w-full text-center">
  <div class="child ">
    <span id="demo" class="span">{timerText}</span>
  </div>
</div>

<style>
  .child {
    background-color: black;
    display: inline-block;
    padding: 10px;
    font-weight: bold;
    font-family: arial;
    color: transparent;
  }

  .span {
    background: url(https://i.ibb.co/gVW2zGL/Farve.jpg);
    background-position: center;
    font-family: "Red Hat Mono", monospace;
    background-size: 100%;
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    display: block;
    font-size: 12.5vw;
  }
</style>
