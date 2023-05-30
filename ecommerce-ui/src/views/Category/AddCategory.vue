<template>
  <div class="container">
    <!--Start of form-->
    <div class="row">
      <!--Center the form-->
      <div class="col-3"></div>
      <div class="col-6">
        <form>
          <!--Header for form starts below-->
          <div class="row">
            <div class="col-12 text-center">
              <h3 class="pt-2">Add Category</h3>
            </div>
          </div>

          <div class="form-group">
            <label for="">Name</label>
            <input type="text" class="form-control" v-model="categoryName" />
            <!--input form form for category name-->
          </div>

          <div class="form-group">
            <label for=""> Description</label>
            <textarea type="text" class="form-control" v-model="description" />
            <!--input form form for category Description-->
          </div>

          <div class="form-group">
            <label for=""> Image</label>
            <input type="text" class="form-control" v-model="imgUrl" />
            <!--input form form for category image-->
          </div>

          <!--submit button-->
          <button
            type="button"
            class="btn btn-primary btn-lg"
            @click="addCategory"
          >
            Submit
          </button>
        </form>
      </div>
      <div class="col-3"></div>
    </div>
  </div>
</template>

<script>
// const axios = require("axios");

export default {
  data() {
    return {
      categoryName: "",
      description: "",
      imgUrl: "",
    };
  },

  methods: {
    addCategory() {
      console.log(this.categoryName, this.description);
      const newCategory = {
        categoryName: this.categoryName,
        description: this.description,
        imgUrl: this.imgUrl,
      };
    },
  },
};
</script>

<!--styles section-->
<style scoped></style>
