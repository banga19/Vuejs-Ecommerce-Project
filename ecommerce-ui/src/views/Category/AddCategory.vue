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
            <input type="text" class="form-control" />
            <!--input form form for category name-->
          </div>

          <div class="form-group">
            <label for=""> Description</label>
            <input type="text" class="form-control" />
            <!--input form form for category Description-->
          </div>

          <div class="form-group">
            <label for=""> Image</label>
            <input type="text" class="form-control" />
            <!--input form form for category image-->
          </div>

          <button type="submit"></button>
        </form>
      </div>
      <div class="col-3"></div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {},
};
</script>

<!--styles section-->
<style scoped></style>
