<template>
  <div>
    <VueColorPickerBoard :width="800" :height="100" :defaultColor="'#00AAFF'">
    </VueColorPickerBoard>
  </div>
</template>

<script>
import VueColorPickerBoard from "vue-color-picker-board";

export default {
  components: {
    VueColorPickerBoard,
  },
};
</script>
