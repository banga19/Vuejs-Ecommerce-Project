<template>
  <div class="card">
    <div>
      <img
        :src="ListCategories.imgUrl"
        alt="Card Image Top"
        class="card-img-top"
      />
    </div>
    <div class="card-body">
      <h5 class="card-title">{{ ListCategories.categoryName }}</h5>
      <p class="card-text">{{ ListCategories.description }}</p>
    </div>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</template>

<script>
export default {
  name: "CategoryBox",
  props: ["ListCategories"],
  methods: {},
};
</script>
