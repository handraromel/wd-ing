<template>
  <div id="wd-header">
    <div class="container pb-md-0">
      <div
        id="header-content"
        class="row justify-content-center align-items-lg-center pt-5"
      >
        <div class="col-xl-6 text-center px-sm-5 px-3 pt-lg-0">
          <!-- <img
            class="img-fluid"
            src="@/assets/img/headec1.png"
            alt="Decoration 1"
            draggable="false"
          /> -->
          <v-lazy-image
            class="img-fluid"
            src="https://annissa-handra.my.id/assets/img/headec1.png"
          />
          <div class="pt-4 pb-0">
            <p class="fs-5 mb-1">Dear Mr. / Mrs. / Ms.</p>
            <p class="dancing guestname">{{ guestName }}</p>
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
          <!-- <img
            class="img-fluid rounded shadow-lg"
            src="@/assets/img/mainfront.webp"
            alt="Sample Photo"
            draggable="false"
          /> -->
          <v-lazy-image
            class="img-fluid rounded shadow-lg"
            src="https://annissa-handra.my.id/assets/img/mainfront.webp"
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
            <!-- <img
              class="img-fluid"
              src="@/assets/img/headec3.png"
              alt="Decoration 3"
              draggable="false"
            /> -->
            <v-lazy-image
              class="img-fluid"
              src="https://annissa-handra.my.id/assets/img/headec3.png"
            />
          </div>
          <div class="dec-loc">
            <!-- <img
              class="img-fluid"
              src="@/assets/img/headec4.png"
              alt="Decoration 4"
              draggable="false"
            /> -->
            <v-lazy-image
              class="img-fluid"
              src="https://annissa-handra.my.id/assets/img/headec4.png"
            />
          </div>
        </div>
        <div class="col-xl-6 text-center pt-about mt-5">
          <!-- <a
            href="javascript:;"
            @click="openFancyBox"
            class="fajardo"
            style="color: inherit"
          >
            <span class="gallery-trig">Catch a glimpse of our moments</span>
          </a> -->
          <span class="fs-6">&#169;&nbsp;2022 Annissa &amp; Handra</span>
        </div>
      </div>
    </div>
    <!-- <FloatBtn /> -->
    <Invitation ref="changeVal" />
  </div>
</template>

<script>
// import FloatBtn from "./FloatBtn.vue";
import Invitation from "./Invitation.vue";
import VLazyImage from "v-lazy-image";

export default {
  data() {
    return {
      guestName: "",
      show: false,
    };
  },
  components: {
    VLazyImage,
    // FloatBtn,
    Invitation,
  },
  methods: {
    openOverlay() {
      document.getElementById("modalOverlay").style.width = "100%";
      this.$refs.changeVal.changeShowedVal();
    },
  },
  mounted() {
    this.guestName = new URL(location.href).searchParams.get("guest");

    var background = document.getElementById("wd-header");

    // Fix background image jump on mobile
    if (
      /Android|iPhone|iPad|iPod|BlackBerry/i.test(
        navigator.userAgent || navigator.vendor || window.opera
      )
    ) {
      background.style.top = "auto";
      background.style.bottom = 0;

      window.onresize = sizeBackground;
      sizeBackground();
    }

    function sizeBackground() {
      background.style.height = screen.height;
    }
  },
};
</script>

<style lang="scss" scoped>
$shadowRadius: 1px 5px 15px #7c6a5e;
$baseColor: #7c6a5e;
$whiteText: #fff;
$buttonPadding: 0.4em 3em;

#wd-header {
  background: url(https://annissa-handra.my.id/assets/img/bg2.webp) center
    no-repeat;
  background-size: cover;
}

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
  font-size: 3.7em;
}

.guestname {
  font-size: 2.3em;
}

// .gallery-trig {
//   font-size: 2.3em;
//   transition: 0.3s;
//   text-shadow: 1px 5px 15px #ab57ff8d;
//   &:hover {
//     text-shadow: $shadowRadius;
//   }
// }

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

@media (max-width: 1399px) {
  .couple-font {
    padding-left: 2em;
    padding-right: 2em;
  }
}

@media (max-width: 1200px) {
  @include headerHeight(85vh);
  @include aboutUsPadding(14em, 5em);

  .couple-font {
    padding-left: 1.5em;
    padding-right: 1.5em;
  }
}

@media (max-width: 992px) {
  .couple-font {
    padding-left: 0;
    padding-right: 0;
  }
}

@media (max-width: 768px) {
  @include decor-position("tape", top, 5%, left, 0, width, 25%);
  @include headerHeight(85vh);

  .bottom-padding {
    padding-bottom: 5em;
  }

  @include aboutUsPadding(7em, 5em);

  .couple-font {
    padding-left: 1.5em;
    padding-right: 1.5em;
  }
}

@media (max-width: 576px) {
  .couple-font {
    padding-left: 0.89em;
    padding-right: 0.89em;
    font-size: 16vw;
  }

  .guestname {
    font-size: 2.5em;
  }
}
</style>
