<template>
  <div class="itemList border d-flex justify-content-between">
    <div class="itemList__info d-flex">
      <div class="itemList__img">
        <img class="border" src="../assets/missing-theme.jpg" alt="place a wait" />
      </div>
      <div class="itemList__name">
        <h5 class="mb-3">{{ scenesData.nameScenes }}</h5>
        <button
          type="button"
          class="btn btn-primary"
          v-for="(group, index) in scenesData.nameGroup"
          :key="index"
        >
          name of group
        </button>
      </div>
    </div>
    <div class="itemList__buttonEdit align-self-end">
      <button type="button" class="btn btn-primary">Edit</button>
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
