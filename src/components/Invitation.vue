<template>
  <div id="modalOverlay" class="overlay">
    <a href="javascript:void(0)" class="closebtn" @click="closeOverlay"
      >&times;</a
    >
    <div class="overlay-content container">
      <section id="sec1">
        <h1>The Bride &amp; Groom</h1>
        <div class="text-white">
          <q
            >I would rather spend one lifetime with you, than face all the ages
            of this world alone.</q
          >
          <p class="fst-italic fw-bold">J.R.R. Tolkien</p>
        </div>
        <div class="row justify-content-center text-center py-md-5">
          <div class="col-md-5 py-3 px-4 px-lg-5 py-md-0">
            <img
              class="img-fluid brides"
              src="@/assets/img/dummy2.png"
              alt=""
              draggable="false"
            />
            <div class="py-4">
              <p class="fs-1 dancing">Annissa Fitri Yonita, S.S.</p>
              <hr>
              <p class="fw-semibold">First daughter of <br> Mr. Erfasyoni <br> &amp; <br> Mrs. Ernisasmita</p>
            </div>
          </div>
          <div class="col-md-2 margin-heart mb-5 mb-md-0">
            <i class="bi bi-hearts"></i>
          </div>
          <div class="col-md-5 py-3 px-4 px-lg-5 py-md-0">
            <img
              class="img-fluid brides"
              src="@/assets/img/dummy1.png"
              alt=""
              draggable="false"
            />
            <div class="py-4">
              <p class="fs-1 dancing">Handra Romel, S.Kom.</p>
              <hr>
              <p class="fw-semibold">First son of <br> Mr. Erwin Romel, S.E. <br> &amp; <br> Mrs. Nurhayati (Almh.)</p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeOverlay() {
      document.getElementById("modalOverlay").style.width = "0%";
    },
  },
};
</script>

<style scoped>
.overlay {
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #9e8673;
  background: #bbb2ab;
  background-image: #9e8673;
  overflow-x: hidden;
  transition: 1s;
  color: rgb(88, 88, 88);
}

.overlay-content {
  position: relative;
  top: 5%;
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

@media (max-width: 1400px) {
}

@media (max-width: 1200px) {
}

@media (max-width: 992px) {
  .margin-heart {
    margin-top: 5em;
  }
}

@media (max-width: 768px) {
  .margin-heart {
    margin-top: 0;
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
    font-size: 2.2em !important;;
  }
}
</style>
