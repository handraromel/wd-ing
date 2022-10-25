<template>
  <div class="floating-container">
    <a
      href="javascript:;"
      class="text-white"
      data-bs-toggle="modal"
      data-bs-target="#giftModal"
    >
      <div class="floating-button">
        <i class="bi bi-gift-fill"></i>
      </div>
      <!-- <div class="floating-text fajardo text-end">
        Send gift
      </div> -->
    </a>
  </div>
  <Gift />
</template>

<script>
import Gift from "./Gift.vue";
export default {
  components: {
    Gift,
  },
};
</script>

<style lang="css" scoped>
.floating-container {
  position: fixed;
  width: 35px;
  height: 35px;
  bottom: 0;
  right: 0;
  margin: 20px 35px;
  z-index: 2;
}

.floating-container:hover .floating-button {
  box-shadow: 0 10px 25px #876f7fbe;
  -webkit-transform: translatey(5px);
  transform: translatey(5px);
  -webkit-transition: all 0.3s;
  transition: all 0.3s;
}

/* .floating-container .floating-text {
  position: absolute;
  bottom: 170%;
  font-size: 1.7em;
  line-height: .6em;
  color: #7c6a5e;
} */

.floating-container .floating-button {
  position: absolute;
  width: 50px;
  height: 50px;
  background: #7c6a5e;
  bottom: 0;
  border-radius: 50%;
  left: 0;
  right: 0;
  margin: auto;
  color: white;
  line-height: 50px;
  text-align: center;
  font-size: 23px;
  z-index: 100;
  box-shadow: 0 10px 25px -5px #7c6a5e8c;
  cursor: pointer;
  -webkit-transition: all 0.3s;
  transition: all 0.3s;
  -webkit-animation: glowing 1s ease-in-out infinite alternate;
  -moz-animation: glowing 1s ease-in-out infinite alternate;
  animation: glowing 1s ease-in-out infinite alternate;
}

@-webkit-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px #876f7f, 0 0 20px #7c6a5e8c,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #876f7f, 0 0 20px #876f7f,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f, 0 0 40 #876f7f;
  }
}
@-moz-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px #876f7f, 0 0 20px #7c6a5e8c,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #876f7f, 0 0 20px #876f7f,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f, 0 0 40 #876f7f;
  }
}
@-o-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px #876f7f, 0 0 20px #7c6a5e8c,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #876f7f, 0 0 20px #876f7f,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f, 0 0 40 #876f7f;
  }
}
@keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px #876f7f, 0 0 20px #7c6a5e8c,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #876f7f, 0 0 20px #876f7f,
      0 0 25px #876f7f, 0 0 30px #876f7f, 0 0 35px #876f7f, 0 0 40 #876f7f;
  }
}

@media (max-width: 1199px) {
  .floating-container {
    margin: 15px 25px;
  }
}
</style>
