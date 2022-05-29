<template>
  <div class="information mb-5">
    <h3 class="font-color mb-4">Diner</h3>

    <div class="information__wrap d-flex">
      <div class="information__img me-5">
        <div class="upload-file mb-3">
          <img class="" src="alo???.pbg" alt="Place upload file" />
        </div>
        <!-- <input type="file" /> -->
        <button type="button" class="btn btn-primary">Upload file</button>
      </div>

      <div class="information__edit">
        <div class="information__edit--name mb-3">
          <label class="font-color me-4">Name: </label>
          <input class="" type="text" placeholder="Name scenes" />
        </div>

        <div class="information__edit--public mb-3">
          <label class="font-color me-4">Public: </label>
          <input class="" type="checkbox" />
        </div>

        <div class="information__edit--group">
          <label class="font-color me-4">Group: </label>
          <select name="" id="">
            <option value="">1</option>
          </select>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
