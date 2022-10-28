<template>
  <div
    class="modal fade"
    id="locModal"
    data-bs-backdrop="static"
    data-bs-keyboard="false"
    tabindex="-1"
    aria-labelledby="locModalLabel"
    aria-hidden="true"
  >
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="locModalLabel">Wedding location</h1>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body p-0">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d249.33825422913543!2d100.6827182!3d-0.8176414!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xc8aad2e268ae8dc6!2zMMKwNDknMDMuNyJTIDEwMMKwNDAnNTcuNyJF!5e0!3m2!1sid!2sid!4v1666945266837!5m2!1sid!2sid"
            width="100%"
            height="450"
            style="border: 0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
#locModal {
  z-index: 2000 !important;
}
</style>
