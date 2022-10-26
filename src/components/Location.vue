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
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d498.67630531881235!2d100.6840383272301!3d-0.8192751840021067!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e2b35b49599a457%3A0x81cda27a23b0ceca!2sperumahan%20villa%20halaban%20indah!5e0!3m2!1sid!2sid!4v1666778087880!5m2!1sid!2sid"
            width="100%"
            height="400"
            frameborder="0"
            style="border: 0"
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
