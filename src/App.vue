<template>
  <div class="row container-scenes mt-5">
    <HelloWorld
      v-for="(item, index) in items"
      :key="index"
      :scenes-data="item"
    />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  components: {
    HelloWorld,
  },

  data() {
    return {
      items: [
        {
          'image': "1.jpg",
          nameScenes: "Breakfast",
          nameGroup: [
            "Linear",
            "Ledstrip",
            "Track White",
            "Single Channel",
            "Track Black",
          ],
        },
        {
          image: "2.jpg",
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
          image: "3.jpg",
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
          image: "4.jpg",
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
          image: "5.jpg",
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
          image: "6.jpg",
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
          image: "7.jpg",
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
