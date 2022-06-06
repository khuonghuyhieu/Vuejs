<template>
  <div class="itemList border d-flex">
    <div class="row itemList__info d-flex">
      <div class="col-2">
        <div class="img-wrap">
          <div class="border itemList__img">
            <img
              class=""
              src="../assets/missing-theme.jpg"
              alt="place a wait"
            />
          </div>
        </div>
      </div>

      <div class="col-7 itemList__name">
        <h5 class="mb-3">{{ scenesData.nameScenes }}</h5>
        <div class="itemList__name--group">
          <label
            class="me-3"
            v-for="(group, index) in scenesData.nameGroup"
            :key="index"
          >
            <i class="text-white">{{ group }}</i>
          </label>
        </div>
      </div>

      <div class="col-3 itemList__buttonEdit align-self-end">
        <button type="button" class="btn btn-primary">Edit</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    scenesData: {
      type: Object,
      required: true,
      default: () => {},
    },
  },

  // props: ["scenesData"] // Nếu k có định dạng thì để nv cũng đc
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
