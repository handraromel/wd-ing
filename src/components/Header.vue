<template>
  <div id="wd-header">
    <div class="container pb-md-0">
      <div
        id="header-content"
        class="row justify-content-center align-items-lg-center pt-5"
      >
        <div class="col-xl-6 text-center px-sm-5 px-3 pt-lg-0">
          <img
            class="img-fluid"
            src="@/assets/img/headec1.png"
            alt="Decoration 1"
            draggable="false"
          />
          <div class="pt-4 pb-0">
            <p class="fs-5 mb-1">Dear Mr. / Mrs. / Ms.</p>
            <h1 class="dancing">{{ guestName }}</h1>
          </div>
          <div class="py-3">
            <p class="mb-1 fs-5">
              We invite you to share in our joy and request <br />
              your presence at the wedding of
            </p>
            <h1 class="pt-2 dancing couple-font" style="letter-spacing: 0.1em">
              Annissa &amp; Handra
            </h1>
          </div>
          <div class="pb-xl-0 pb-5">
            <a
              href="javascript:;"
              class="btn rounded-pill read-more"
              @click="openOverlay"
              >Open Invitation</a
            >
          </div>
        </div>
        <div class="col-xl-6 text-center position-relative px-5">
          <img
            class="img-fluid"
            src="@/assets/img/mainfront.webp"
            alt="Sample Photo"
            draggable="false"
          />
          <!-- <div class="dec-tape">
            <img
              class="img-fluid"
              src="@/assets/img/headec2.png"
              alt="Decoration 2"
              draggable="false"
            />
          </div> -->
          <div class="dec-logo">
            <img
              class="img-fluid"
              src="@/assets/img/headec3.png"
              alt="Decoration 3"
              draggable="false"
            />
          </div>
          <div class="dec-loc">
            <img
              class="img-fluid"
              src="@/assets/img/headec4.png"
              alt="Decoration 4"
              draggable="false"
            />
          </div>
        </div>
        <div class="col-xl-6 text-center pt-about">
          <a
            href="javascript:;"
            @click="openFancyBox"
            class="fajardo"
            style="color: inherit"
          >
            <span class="fs-1">About us</span>
          </a>
        </div>
      </div>
    </div>
    <FloatBtn />
    <Invitation ref="changeVal" />
    <audio id="player" autoplay loop>
      <source src="@/assets/media/audioplayback.mp3" type="audio/mp3" />
    </audio>
  </div>
</template>

<script>
import FloatBtn from "./FloatBtn.vue";
import Invitation from "./Invitation.vue";
import { Fancybox } from "@fancyapps/ui";
import "@fancyapps/ui/dist/fancybox.css";
import PerfectScrollbar from "perfect-scrollbar";

export default {
  data() {
    return {
      guestName: "",
      show: false,
    };
  },
  components: {
    FloatBtn,
    Invitation,
  },
  methods: {
    openOverlay() {
      document.getElementById("modalOverlay").style.width = "100%";
      this.$refs.changeVal.changeShowedVal();
    },
    openFancyBox() {
      Fancybox.show([
        { src: "src/assets/img/1.jpg", type: "image" },
        { src: "src/assets/img/2.jpg", type: "image" },
        { src: "src/assets/img/3.jpg", type: "image" },
        { src: "src/assets/img/4.jpg", type: "image" },
        { src: "src/assets/img/5.jpg", type: "image" },
        { src: "src/assets/img/6.jpg", type: "image" },
        { src: "src/assets/img/7.jpg", type: "image" },
        { src: "src/assets/img/8.jpg", type: "image" },
        { src: "src/assets/img/9.jpg", type: "image" },
        { src: "src/assets/img/10.jpg", type: "image" },
        { src: "src/assets/img/11.jpg", type: "image" },
        { src: "src/assets/img/12.jpg", type: "image" },
      ]);
    },
  },
  mounted() {
    this.guestName = new URL(location.href).searchParams.get("guest");
    const ps = new PerfectScrollbar("#wd-header");
    var vid = document.getElementById("player");
    vid.volume = 0.5;
  },
};
</script>

<style lang="scss" scoped>
$assetsPath: "@/assets/img";
$shadowRadius: 1px 5px 15px #7c6a5e;
$baseColor: #7c6a5e;
$whiteText: #fff;
$buttonPadding: 0.4em 3em;

.read-more {
  background: $baseColor;
  color: $whiteText;
  border: none;
  padding: $buttonPadding;
  letter-spacing: 0.3em;
  &:hover,
  &:active,
  &:focus {
    box-shadow: $shadowRadius;
    background: $baseColor;
    color: $whiteText;
  }
}

@mixin decor-position(
  $name,
  $top-or-bottom,
  $x,
  $left-or-right,
  $y,
  $img-width,
  $width
) {
  .dec-#{$name} {
    position: absolute;
    #{$top-or-bottom}: $x;
    #{$left-or-right}: $y;
    #{$img-width}: $width;
  }
}

.couple-font {
  font-size: 4em;
}

@mixin headerHeight($height) {
  #header-content {
    min-height: $height;
  }
}

@mixin aboutUsPadding($pt, $pb) {
  .pt-about {
    padding-top: $pt;
    padding-bottom: $pb;
  }
}

@include headerHeight(100vh);

// @include decor-position("tape", top, 0, left, 0, width, 25%);
@include decor-position("logo", top, 5%, right, 0, width, 30%);
@include decor-position("loc", bottom, -30%, right, 15%, width, 55%);

@media (max-width: 1200px) {
  @include headerHeight(85vh);
  @include aboutUsPadding(14em, 5em);
}

@media (max-width: 760px) {
  @include decor-position("tape", top, 5%, left, 0, width, 25%);
  @include headerHeight(85vh);

  .bottom-padding {
    padding-bottom: 5em;
  }

  @include aboutUsPadding(7em, 5em);
}
</style>
