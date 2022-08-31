<template>
  <header id="wd-header">
    <div class="container">
      <div class="row align-items-center vh-100">
        <div class="col-md-6 text-center">
          <img
            class="img-fluid"
            src="@/assets/img/headec1.png"
            alt="Decoration 1"
            draggable="false"
          />
          <div class="py-5">
            <h1 class="fw-bold">Lorem The Ipsum</h1>
            <h3 style="letter-spacing: 0.4em">Lorem &amp; Ipsum</h3>
          </div>
          <a href="javascript:;" class="btn rounded-pill read-more"
            >READ MORE</a
          >
          <div class="py-5">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean non
            dignissim neque. Phasellus ullamcorper libero tellus, in aliquet
            elit placerat interdum. Vivamus porttitor turpis neque, et porttitor
            massa mollis non. Curabitur ac tincidunt nulla. Suspendisse finibus
            eros ut felis eleifend, quis ultricies felis posuere.
          </div>
        </div>
        <div class="col-md-6 text-center position-relative p-5">
          <img
            class="img-fluid"
            src="@/assets/img/sample.webp"
            alt="Sample Photo"
            draggable="false"
          />
          <div class="dec2">
            <img
              class="img-fluid"
              src="@/assets/img/headec2.png"
              alt="Decoration 2"
              draggable="false"
            />
          </div>
          <div class="dec3">
            <img
              class="img-fluid"
              src="@/assets/img/headec3.png"
              alt="Decoration 3"
              draggable="false"
            />
          </div>
          <div class="dec4">
            <img
              class="img-fluid"
              src="@/assets/img/headec4.png"
              alt="Decoration 4"
              draggable="false"
            />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
$assetsPath: "@/assets/img";
$shadowRadius: 1px 5px 15px #7c6a5e;
$baseColor: #7c6a5e;
$whiteText: #fff;
$buttonPadding: 0.4em 3em;

#wd-header {
  background: url(#{$assetsPath}/header-bg.webp) center no-repeat;
  background-size: cover;
  // min-height: 100vh;
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

// @mixin decor-position($name, $top-or-bottom, $left-or-right, $img-width) {
//   .dec-#{$name} {
//     position: absolute;
//     #{$top-or-bottom} : 0;
//     #{$left-or-right} : 0;
//     #{$img-width} : 0;
//   }
// }

// @include decor-position("tape", top, left, width);

.dec2 {
  position: absolute;
  top:0;
  left: 0;
  width: 25%;
}

.dec3 {
  position: absolute;
  top:15%;
  right: 0;
  width: 30%;
}

.dec4 {
  position: absolute;
  bottom:-20%;
  right: 15%;
  width: 55%;
}
</style>