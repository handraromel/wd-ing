<template>
  <div id="modalOverlay" class="overlay">
    <a href="javascript:void(0)" class="closebtn" @click="closeOverlay"
      >&times;</a
    >
    <transition>
      <div v-show="showed" class="overlay-content">
        <section id="sec1">
          <div class="container">
            <div id="">
              <h1 class="sunflower">The Bride &amp; Groom</h1>
              <div class="text-white">
                <q
                  >I would rather spend one lifetime with you, than face all the
                  ages of this world alone.</q
                >
                <p class="fst-italic fw-bold">J.R.R. Tolkien</p>
              </div>
              <div class="row justify-content-center text-center py-md-5">
                <div class="col-md-5 py-3 px-4 px-lg-5 py-md-0">
                  <div class="px-xl-5 px-md-2 px-5">
                    <img
                      class="img-fluid brides"
                      src="@/assets/img/top-l.webp"
                      alt=""
                      draggable="false"
                    />
                  </div>
                  <div class="py-4">
                    <p class="fs-1 dancing">Annissa Fitri Yonita, S.S.</p>
                    <hr />
                    <p>
                      First daughter of <br />
                      <span class="megalona fw-bold">Mr. Erfasyoni</span>
                      <br />
                      <span class="fw-bold">&amp;</span> <br />
                      <span class="megalona fw-bold">Mrs. Ernisasmita</span>
                    </p>
                  </div>
                </div>
                <div class="col-md-2 margin-heart mb-5 mb-md-0">
                  <i class="bi bi-hearts"></i>
                </div>
                <div class="col-md-5 py-3 px-4 px-lg-5 py-md-0">
                  <div class="px-xl-5 px-md-2 px-5">
                    <img
                      class="img-fluid brides"
                      src="@/assets/img/top-r.webp"
                      alt=""
                      draggable="false"
                    />
                  </div>
                  <div class="py-4">
                    <p class="fs-1 dancing">Handra Romel, S.Kom.</p>
                    <hr />
                    <p>
                      First son of <br />
                      <span class="megalona fw-bold"
                        >Mr. Erwin Romel, S.E.</span
                      >
                      <br />
                      <span class="fw-bold">&amp;</span> <br />
                      <span class="megalona fw-bold"
                        >Mrs. Nurhayati (Almh.)</span
                      >
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <section id="sec2">
          <div id="trigger1"></div>
          <div class="container">
            <div id="reveal1" class="ins-container">
              <div class="titleset d-flex justify-content-center">
                <div class="align-self-end text-white mb-5">
                  <h1 class="sunflower">Wedding Day</h1>
                  <h5>Location &amp; Time</h5>
                </div>
              </div>
              <div class="contentset py-5">
                <div class="row justify-content-center align-items-center">
                  <div class="col-md-5 px-sm-4 px-5 py-4">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                      version="1.1"
                      id="Layer_1"
                      x="0px"
                      y="0px"
                      viewBox="0 0 512 512"
                      style="enable-background: new 0 0 512 512"
                      xml:space="preserve"
                      width="70px"
                      height="70px"
                    >
                      <g>
                        <path
                          style="fill: #ffe6b9"
                          d="M232.13,154.172c-4.56,3.825-8.816,8.001-12.717,12.495C277.724,185.083,320,239.602,320,304
		c0,16.727-2.862,32.783-8.106,47.718c6.02-0.421,11.912-1.316,17.635-2.656c4.204-14.3,6.471-29.42,6.471-45.062
		C336,235.519,292.747,176.957,232.13,154.172z"
                        />
                        <path
                          style="fill: #ebd2aa"
                          d="M277.728,381.59C254.318,412.208,217.429,432,176,432c-70.578,0-128-57.422-128-128
		c0-70.252,56.894-127.46,127.024-127.988c2.722-5.464,5.778-10.732,9.146-15.777C181.466,160.084,178.743,160,176,160
		c-79.529,0-144,64.471-144,144c0,79.529,64.471,144,144,144c50.025,0,94.085-25.513,119.897-64.232
		C289.73,383.424,283.666,382.689,277.728,381.59z"
                        />
                        <polygon
                          style="fill: #82c8dc"
                          points="272,37.241 232,37.241 268.471,80 288.209,80 	"
                        />
                        <polygon
                          style="fill: #b4e6f0"
                          points="319.791,80 339.529,80 376,37.241 336,37.241 	"
                        />
                        <polygon
                          style="fill: #d9ffff"
                          points="304,37.241 336,37.241 304,0 272,37.241 	"
                        />
                        <polygon
                          style="fill: #a0dce6"
                          points="304,37.241 272,37.241 288.209,80 304,80 319.791,80 336,37.241 	"
                        />
                        <polygon
                          style="fill: #a0dce6"
                          points="264.276,0 232,37.241 272,37.241 	"
                        />
                        <polygon
                          style="fill: #ebffff"
                          points="376,37.241 343.724,0 336,37.241 	"
                        />
                        <polygon
                          style="fill: #b4e6f0"
                          points="343.724,0 304,0 336,37.241 	"
                        />
                        <polygon
                          style="fill: #b4e6f0"
                          points="304,0 264.276,0 272,37.241 	"
                        />
                        <path
                          style="fill: #ffe6b9"
                          d="M448,240c0-64.262-42.314-118.82-100.542-137.292L352,80h-12.471h-19.739H304v32
		c70.581,0,128,57.419,128,128c0,70.58-57.419,128-128,128s-128-57.42-128-128c0-56.506,36.806-104.57,87.701-121.495l-3.159-15.797
		c-25.365,8.047-47.707,22.941-64.85,42.505C189.237,144.417,182.666,144,176,144c-88.223,0-160,71.777-160,160s71.777,160,160,160
		c59.266,0,111.11-32.392,138.758-80.401C389.155,378.078,448,315.784,448,240z M176,448c-79.529,0-144-64.471-144-144
		c0-79.529,64.471-144,144-144c2.743,0,5.466,0.084,8.171,0.235c-3.369,5.044-6.425,10.313-9.146,15.777
		C165.416,195.3,160,217.028,160,240c0,70.431,50.828,129.207,117.728,141.59c5.938,1.099,12.002,1.833,18.169,2.177
		C270.085,422.487,226.025,448,176,448z"
                        />
                        <path
                          style="fill: #ebd2aa"
                          d="M176,240c0,70.58,57.419,128,128,128s128-57.42,128-128c0-70.581-57.419-128-128-128V80h-15.791
		h-19.739H256l4.542,22.708l3.159,15.797C212.806,135.43,176,183.494,176,240z M192,240c0-21.896,6.322-42.342,17.227-59.617
		C263.748,195.053,304,244.911,304,304c0,16.822-3.268,32.893-9.193,47.62C237.334,346.929,192,298.662,192,240z M416,240
		c0,52.978-36.973,97.479-86.471,109.062c-5.723,1.339-11.615,2.235-17.635,2.656C317.138,336.783,320,320.727,320,304
		c0-64.398-42.276-118.917-100.586-137.333c3.901-4.494,8.157-8.669,12.717-12.495C251.595,137.847,276.667,128,304,128
		C365.758,128,416,178.242,416,240z"
                        />
                      </g>
                    </svg>
                    <h2>Akad Nikah</h2>
                    <hr />
                    <div class="text-start">
                      <table>
                        <tr>
                          <td><i class="bi bi-calendar"></i></td>
                          <td>Saturday, 3 December 2022</td>
                        </tr>
                        <tr>
                          <td><i class="bi bi-clock"></i></td>
                          <td>08.00 &mdash; 10.00</td>
                        </tr>
                        <tr>
                          <td><i class="bi bi-geo-alt-fill"></i></td>
                          <td>
                            Perumnas Halaban Tahap III, Blok BB 19, Nagari
                            Panyakalan, Kubung, Solok, Sumatera Barat
                          </td>
                        </tr>
                      </table>
                    </div>
                  </div>
                  <div class="col-md-5 px-sm-4 px-5 py-4">
                    <svg
                      version="1.1"
                      id="Capa_1"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                      x="0px"
                      y="0px"
                      viewBox="0 0 456 456"
                      style="enable-background: new 0 0 456 456"
                      xml:space="preserve"
                      width="70px"
                      height="70px"
                    >
                      <g>
                        <path
                          style="fill: #faeee2"
                          d="M232,60c-92.784,0-168,75.216-168,168c0,92.784,75.216,168,168,168s168-75.216,168-168
		C400,135.216,324.784,60,232,60z M232,340c-61.759,0-112-50.241-112-112s50.241-112,112-112s112,50.241,112,112
		S293.759,340,232,340z"
                        />
                        <path
                          style="fill: #ffebe1"
                          d="M232,132c-52.935,0-96,43.065-96,96s43.065,96,96,96s96-43.065,96-96S284.935,132,232,132z"
                        />
                        <path
                          style="fill: #ffdcaa"
                          d="M232,116c-61.759,0-112,50.241-112,112s50.241,112,112,112s112-50.241,112-112S293.759,116,232,116z
		 M232,324c-52.935,0-96-43.065-96-96s43.065-96,96-96s96,43.065,96,96S284.935,324,232,324z"
                        />
                        <path
                          style="fill: #f5e1d2"
                          d="M43.2,84c-2.651,0-4.8,2.217-4.8,4.952v69.333c0,2.735-2.149,4.952-4.8,4.952
		c-2.651,0-4.8-2.217-4.8-4.952V88.952C28.8,86.217,26.651,84,24,84s-4.8,2.217-4.8,4.952v69.333c0,2.735-2.149,4.952-4.8,4.952
		c-2.651,0-4.8-2.217-4.8-4.952V88.952C9.6,86.217,7.451,84,4.8,84C2.149,84,0,86.217,0,88.952v79.238
		c0,9.293,6.227,17.034,14.594,19.171L8.571,356.01C8.259,364.747,15.257,372,24,372s15.741-7.253,15.429-15.99l-6.023-168.648
		C41.773,185.225,48,177.484,48,168.19V88.952C48,86.217,45.851,84,43.2,84z"
                        />
                        <path
                          style="fill: #f5e1d2"
                          d="M447.372,84c-4.245,0-7.86,3.089-8.522,7.282l-20.736,131.33
		c-1.22,7.726,3.325,15.201,10.745,17.674L440,244l-13.892,111.135C424.989,364.09,431.971,372,440.996,372l0,0
		c8.286,0,15.004-6.718,15.004-15.004V92.628C456,87.863,452.137,84,447.372,84z"
                        />
                      </g>
                    </svg>
                    <h2>Wedding Reception</h2>
                    <hr />
                    <div class="text-start">
                      <table>
                        <tr>
                          <td><i class="bi bi-calendar"></i></td>
                          <td>Saturday, 3 December 2022</td>
                        </tr>
                        <tr>
                          <td><i class="bi bi-clock"></i></td>
                          <td>10.00 &mdash; done</td>
                        </tr>
                        <tr>
                          <td><i class="bi bi-geo-alt-fill"></i></td>
                          <td>
                            Perumnas Halaban Tahap III, Blok BB 19, Nagari
                            Panyakalan, Kubung, Solok, Sumatera Barat
                          </td>
                        </tr>
                      </table>
                    </div>
                  </div>
                  <div class="col-12">
                    <a
                      href="javascript:;"
                      class="btn rounded-pill loc-btn"
                      data-bs-toggle="modal"
                      data-bs-target="#locModal"
                      >Open in Google Map</a
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <section id="sec3">
          <div class="container">
            <div class="ins-container">
              <div class="pb-5">
                <h5>This event will be held using</h5>
                <h1 class="sunflower">Health Protocol</h1>
                <h5>
                  in accordance with government regulations &amp;
                  recommendations
                </h5>
              </div>
              <div id="trigger2"></div>
              <div id="reveal2" class="row protocols">
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/mask.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">Wear Mask</p>
                </div>
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/soap.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">Use Soap</p>
                </div>
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/wash.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">Wash Hands</p>
                </div>
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/crowd.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">Avoid the Crowds</p>
                </div>
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/sanitizer.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">Use Hand Sanitizer</p>
                </div>
                <div class="col-md-4 col-6 p-4">
                  <img
                    class="img-fluid"
                    src="@/assets/img/hands.png"
                    alt=""
                    draggable="false"
                  />
                  <p class="py-3">No Handshake</p>
                </div>
              </div>
            </div>
          </div>
        </section>
        <section id="sec4" class="text-white">
          <div class="container">
            <div class="ins-container">
              <div id="trigger3"></div>
              <div id="reveal3" class="row align-items-center">
                <h3>Thank You</h3>
                <p class="pb-3 bottom-name dancing">Annissa &amp; Handra</p>
                <p class="fw-bold" style="line-height: 1.2em">
                  The Big Family of
                </p>
                <p style="line-height: 0.4em">
                  Mr. Erfasyoni &amp; Mrs. Ernisasmita
                </p>
                <p style="line-height: 1.2em">
                  Mr. Erwin Romel, S.E. &amp; Mrs. Nurhayati (Almh.)
                </p>
              </div>
            </div>
          </div>
        </section>
      </div>
    </transition>
  </div>
  <Location />
</template>

<script>
import ScrollMagic from "scrollmagic";
import PerfectScrollbar from "perfect-scrollbar";
import Location from "./Location.vue";
export default {
  components: {
    Location,
  },
  data() {
    return {
      controller: null,
      scene1: null,
      scene2: null,
      scene3: null,
      showed: false,
    };
  },
  methods: {
    closeOverlay() {
      document.getElementById("modalOverlay").style.width = "0%";
      this.showed = false;
    },
    changeShowedVal() {
      this.showed = true;
    },
    scrollMagicTrig() {
      this.controller = new ScrollMagic.Controller();
      this.scene1 = new ScrollMagic.Scene({
        triggerElement: "#trigger1",
        triggerHook: 0.5,
      })
        .setClassToggle("#reveal1", "visible")
        .addTo(this.controller);
      this.scene2 = new ScrollMagic.Scene({
        triggerElement: "#trigger2",
        triggerHook: 0.9,
      })
        .setClassToggle("#reveal2", "visible")
        .addTo(this.controller);
      this.scene3 = new ScrollMagic.Scene({
        triggerElement: "#trigger3",
        triggerHook: 0.9,
      })
        .setClassToggle("#reveal3", "visible")
        .addTo(this.controller);
    },
  },
  mounted() {
    this.scrollMagicTrig();
    const ps = new PerfectScrollbar("#modalOverlay");
  },
};
</script>

<style scoped>
.v-enter-active {
  transition: opacity 4s ease;
}
.v-leave-active {
  transition: opacity 0.2s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}

.overlay {
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #bbb2ab;
  background: #bbb2ab;
  background-image: #bbb2ab;
  overflow-x: hidden;
  transition: 1s;
  color: rgb(88, 88, 88);
}

#sec2 {
  background-color: #bbb2ab;
  background: url("@/assets/img/bg2.webp") center no-repeat;
  background-image: #bbb2ab;
  background-size: cover;
}

#sec3 {
  background-color: #bbb2ab;
  background: #bbb2ab;
  background-image: #bbb2ab;
}

#sec4 {
  background-color: #bbb2ab;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("@/assets/img/foot.webp") center no-repeat;
  background-image: #bbb2ab;
  background-size: cover;
  min-height: 75vh;
  padding-top: 7.5em;
}

.overlay-content {
  position: relative;
  top: 5.5%;
  width: 100%;
  text-align: center;
  margin-top: 30px;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 36px;
  color: #818181;
  display: block;
  transition: 0.3s;
}

.overlay a:hover,
.overlay a:focus {
  color: #f1f1f1;
}

.overlay .closebtn {
  position: absolute;
  top: 0%;
  right: 2%;
  font-size: 50px;
  color: #615247;
}

.brides {
  border-radius: 5em;
}

.bi-hearts {
  font-size: 3em;
  text-shadow: 1px 1px 15px #615247;
}

.margin-heart {
  margin-top: 11em;
}

.titleset {
  background-color: #bbb2ab;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url("@/assets/img/bg-mid.webp") center no-repeat;
  background-image: #bbb2ab;
  height: 300px;
  border-top-left-radius: 2em;
  border-top-right-radius: 2em;
  background-size: cover;
  background-position-y: -130px;
}

.contentset {
  background-color: #bbb2ab;
  background: #bbb2ab;
  background-image: #bbb2ab;
  border-bottom-left-radius: 2em;
  border-bottom-right-radius: 2em;
}

.ins-container {
  padding: 5em 0;
}

.protocols {
  padding: 0 10em;
}

.bottom-name {
  font-size: 4.5em;
  padding: 0 1.15em;
}

table td,
table td * {
  vertical-align: top;
}

td {
  padding: 0.2em;
}

#reveal1,
#reveal2,
#reveal3 {
  opacity: 0;
  -webkit-transform: translateY(10%);
  -moz-transform: translateY(10%);
  -ms-transform: translateY(10%);
  -o-transform: translateY(10%);
  transform: translateY(10%);
  -webkit-transition: all 0.8s ease-in-out;
  -moz-transition: all 0.8s ease-in-out;
  -ms-transition: all 0.8s ease-in-out;
  -o-transition: all 0.8s ease-in-out;
  transition: all 0.8s ease-in-out;
}

#reveal1.visible,
#reveal2.visible,
#reveal3.visible {
  opacity: 1;
  -webkit-transform: none;
  -moz-transform: none;
  -ms-transform: none;
  -o-transform: none;
  transform: none;
}

/* .loc-btn {
  background: #7c6a5e;
  color: #fff;
  border: none;
  padding: ;
  letter-spacing: 0.3em;
} */

a.loc-btn {
  text-decoration: none !important;
  background: #7c6a5e;
  padding: 0.3em 1.5em;
  text-align: center;
  transition: 0.5s;
  color: #ffffff;
  font-size: 1em;
  border: 0;
  margin-top: 2em;
  border-radius: 0;
  z-index: 1;
  display: inline-block;
}

a.loc-btn:hover {
  box-shadow: 0 0 10px #7c6a5e;
}

@media (max-width: 1400px) {
  #sec4 {
    padding-top: 0.5em;
  }
}

@media (max-width: 1200px) {
  #sec4 {
    padding-top: 0.5em;
  }
}

@media (max-width: 992px) {
  .margin-heart {
    margin-top: 5em;
  }

  .protocols {
    padding: 0;
  }

  .titleset {
    background-position-y: -100px;
  }

  #sec4 {
    padding-top: 8em;
  }
}

@media (max-width: 768px) {
  .margin-heart {
    margin-top: 0;
  }

  .titleset {
    background-position-y: -10px;
  }
}

@media (max-width: 576px) {
  .overlay a {
    font-size: 20px;
  }
  .overlay .closebtn {
    font-size: 40px;
  }

  .margin-heart {
    margin-top: 0;
  }

  .fs-1 {
    font-size: 2.2em !important;
  }

  .titleset {
    background-position-y: 0px;
  }

  #sec4 {
    padding-top: 0.5em;
  }
}
</style>
