<template>
  <div class="app">
    <!-- <HelloWorld
      v-for="(item, index) in items"
      :key="index"
      :scenes-data="item"
    /> -->
    <!-- <LayoutEdit /> -->
    <!-- <ColorPicker /> -->
    <!-- <VueColorPickerBoard :width="800" :height="100" :defaultColor="'#00AAFF'">
    </VueColorPickerBoard> -->
    <!-- <Test></Test> -->
    <div class="row">
      <div class="col-3"></div>
      <div class="col-9">
        <div class="label-wrap">
          <label class="me-3 text-white">{{ displayedText }}</label>
        </div>
        <div v-if="groups.length > 20" class="view-all" @click="showFullText = !showFullText">
          ...Read {{ viewAll }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import LayoutEdit from "./components/layout-edit.vue";
// import ColorPicker from "./components/color-picker.vue";
// import VueColorPickerBoard from "vue-color-picker-board";
// import Test from "./components/learn-vue.vue";
export default {
  data() {
    return {
      isShowButton: false,
      name: false,
      showFullText: false,

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

      groups: [
        "Hiếu",
        "Khương",
        "Huy",
        "Thư",
        "Lưu",
        "Name",
      ],
    };
  },

  components: {
    // HelloWorld,
    // LayoutEdit,
    // ColorPicker,
    // VueColorPickerBoard,
    // Test
  },

  computed: {
    displayedText() {
      if (!this.showFullText) {
        return this.groups.slice(0, 20).join(', ');
      } else {
        return this.groups.join(', ');
      }
    },

   viewAll(){
     return this.showFullText ? 'close' : 'more';
   },

  },

  methods: {
  //   showReadMore(){
  //    if(this.groups.length < 20){
  //      console.log("aaaaaa");
  //      this.showMoreGroup = true;
  //    }
  //  },

    showName() {
      console.log(this.name);
      this.name = true;
    },
  },
};
</script>

<style></style>
