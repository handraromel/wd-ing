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
}

.floating-container:hover .floating-button {
  box-shadow: 0 10px 25px rgba(44, 179, 240, 0.6);
  -webkit-transform: translatey(5px);
  transform: translatey(5px);
  -webkit-transition: all 0.3s;
  transition: all 0.3s;
}

.floating-container .floating-button {
  position: absolute;
  width: 50px;
  height: 50px;
  background: #2cb3f0;
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
  box-shadow: 0 10px 25px -5px rgba(44, 179, 240, 0.6);
  cursor: pointer;
  -webkit-transition: all 0.3s;
  transition: all 0.3s;
  -webkit-animation: glowing 1s ease-in-out infinite alternate;
  -moz-animation: glowing 1s ease-in-out infinite alternate;
  animation: glowing 1s ease-in-out infinite alternate;
}

@-webkit-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px rgba(255, 0, 255, 0.466), 0 0 20px rgba(0, 255, 255, 0.452),
      0 0 25px #e6007379, 0 0 30px #e600737a, 0 0 35px #e6007379;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #ff4da683, 0 0 20px #ff4da681,
      0 0 25px #ff4da68a, 0 0 30px #ff4da68a, 0 0 35px #ff4da688, 0 0 40 rgba(255, 77, 166, 0.527);
  }
}
@-moz-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px rgba(255, 0, 255, 0.466), 0 0 20px rgba(0, 255, 255, 0.452),
      0 0 25px #e6007379, 0 0 30px #e600737a, 0 0 35px #e6007379;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #ff4da683, 0 0 20px #ff4da681,
      0 0 25px #ff4da68a, 0 0 30px #ff4da68a, 0 0 35px #ff4da688, 0 0 40 rgba(255, 77, 166, 0.527);
  }
}
@-o-keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px rgba(255, 0, 255, 0.466), 0 0 20px rgba(0, 255, 255, 0.452),
      0 0 25px #e6007379, 0 0 30px #e600737a, 0 0 35px #e6007379;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #ff4da683, 0 0 20px #ff4da681,
      0 0 25px #ff4da68a, 0 0 30px #ff4da68a, 0 0 35px #ff4da688, 0 0 40 rgba(255, 77, 166, 0.527);
  }
}
@keyframes glowing {
  from {
    box-shadow: 0 0 5px rgba(255, 255, 255, 0.5), 0 0 10px rgba(255, 255, 255, 0.7), 0 0 15px rgba(255, 0, 255, 0.466), 0 0 20px rgba(0, 255, 255, 0.452),
      0 0 25px #e6007379, 0 0 30px #e600737a, 0 0 35px #e6007379;
  }
  to {
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.5), 0 0 15px #ff4da683, 0 0 20px #ff4da681,
      0 0 25px #ff4da68a, 0 0 30px #ff4da68a, 0 0 35px #ff4da688, 0 0 40 rgba(255, 77, 166, 0.527);
  }
}

@media (max-width: 1199px) {
  .floating-container {
    margin: 15px 25px;
  }
}
</style>
