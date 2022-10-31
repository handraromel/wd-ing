<template>
  <audio id="player" controls loop style="display: none">
    <source
      src="https://annissa-handra.my.id/assets/media/audioplayback.mp3"
      type="audio/mpeg"
    />
  </audio>
  <div></div>
</template>

<script>
export default {
  mounted() {
    var audio = document.getElementById("player");
    audio.volume = 0.3;

    audio.addEventListener("canplaythrough", () => {
      audio.play().catch((e) => {
        window.addEventListener(
          "click",
          () => {
            audio.play();
          },
          { once: true }
        );
      });
    });
  },
};
</script>
