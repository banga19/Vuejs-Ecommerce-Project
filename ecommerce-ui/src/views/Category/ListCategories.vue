<template>
  <div class="container">
    <div class="row">
      <div class="col-12 text-center">
        <h3 class="pt-3">Our Categories</h3>
        <div>{{ ListCategories }}</div>
      </div>
      <div class="row"></div>
    </div>
  </div>
</template>

<script>
var axios = require("axios");
//import CategoryBox from "../../components/Category/CategoryBox.vue";

export default {
  name: "ListCategories",
  components: {},
  data() {
    return {
      baseURL: "https://limitless-lake-55070.herokuapp.com/",
      Categories: null,
    };
  },

  methods: {
    async getCategories() {
      // fetch categories
      await axios
        .get(`${this.baseURL} + "ListCategories/"`)
        .then((res) => (this.ListCategories = res.data))
        .catch((err) => console.log(err));
    },
  },
  mounted() {
    this.getCategories();
  },
};
</script>

<!--styles section-->
<style scoped>
h4 {
  font-family: "Roboto", sans-serif;
  color: #484848;
  font-weight: 700;
}
#add-category {
  float: right;
  font-weight: 500;
}
</style>
