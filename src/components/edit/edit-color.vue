<template>
  <div class="col">
    <div class="input-group mb-4">
      <div class="input-group-prepend me-3">
        <div class="input-group-text">
          <input
            class="margin"
            name="checkbox"
            type="radio"
            aria-label="Radio button for following text input"
          />
        </div>
      </div>
      <h5 class="font-color">COLOR SPECIFICATION</h5>
    </div>

    <div class="color-type d-flex">
      <h6 class="font-color me-4">Fusion color type: </h6>
      <div class="checkbox">
        <div class="form-check">
          <input
            class="form-check-input"
            type="radio"
            name="flexRadioDefault"
            id="flexRadioDefault1"
          />
          <label class="form-check-label font-color" for="flexRadioDefault1">
            CCT
          </label>
        </div>
        <div class="form-check">
          <input
            class="form-check-input"
            type="radio"
            name="flexRadioDefault"
            id="flexRadioDefault2"
            checked
          />
          <label class="form-check-label font-color" for="flexRadioDefault2">
            XY
          </label>
        </div>
      </div>
      <!-- <div class="color-type">
        <input type="radio" /> CCT <input type="radio" /> XY
      </div> -->
    </div>
  </div>
</template>

<script>
export default {};
</script>
