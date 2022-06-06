<template>
  <div class="app">
    <HelloWorld
      v-for="(item, index) in items"
      :key="index"
      :scenes-data="item"
    />
    <!-- <LayoutEdit /> -->
    <!-- <ColorPicker /> -->
    <!-- <VueColorPickerBoard :width="800" :height="100" :defaultColor="'#00AAFF'">
    </VueColorPickerBoard> -->
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
// import LayoutEdit from "./components/layout-edit.vue";
// import ColorPicker from "./components/color-picker.vue";
// import VueColorPickerBoard from "vue-color-picker-board";
export default {
  components: {
    HelloWorld,
    // LayoutEdit,
    // ColorPicker,
    // VueColorPickerBoard
  },

  data() {
    return {
      items: [
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Breakfast",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Conference",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Dinner",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Lunch",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Meeting",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Party",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "../assets/missing-theme.jpg",
          nameScenes: "Presentation",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
