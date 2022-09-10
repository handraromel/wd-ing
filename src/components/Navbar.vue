<template>
  <nav class="navbar navbar-expand-lg fixed-top bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a
              @click="isActive1 = true"
              :class="{ active: isActive1 }"
              class="nav-link"
              href="#"
              >Home</a
            >
          </li>
          <li class="nav-item">
            <a
              @click="isActive2 = true"
              :class="{ active: isActive2 }"
              class="nav-link"
              href="#"
              >Nav1</a
            >
          </li>
          <li class="nav-item">
            <a
              @click="isActive3 = true"
              :class="{ active: isActive3 }"
              class="nav-link"
              href="#"
              >Nav3</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isActive1: true,
      isActive2: false,
      isActive3: false,
    };
  },
  watch: {
    isActive1(val) {
      if (val === true) {
        this.isActive2 = false;
        this.isActive3 = false;
      }
    },
    isActive2(val) {
      if (val === true) {
        this.isActive1 = false;
        this.isActive3 = false;
      }
    },
    isActive3(val) {
      if (val === true) {
        this.isActive1 = false;
        this.isActive2 = false;
      }
    },
  },
};
</script>

<style scoped>
.active {
  background-color: #7c6a5e;
  transition: 0.5s;
  color: #fff !important;
  font-size: 1em;
  z-index: 1;
}

.nav-link {
  margin-left: 0.5em;
  margin-right: 0.5em;
}

@media (max-width: 992px) {
  .nav-link {
    padding-left: 0.5em;
    padding-right: 0.5em;
    margin-top: 1em;
    margin-left: 0em;
    margin-right: 0em;
  }
}
</style>