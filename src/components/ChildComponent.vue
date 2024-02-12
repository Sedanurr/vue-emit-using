<template>
  <div>
    <div>
      <img src="@/assets/kedii.jpeg" style="width: 50%; height: 100%" />
      <p>Cats</p>
    </div>

    <div>
      <button @click="addCat">Ekle</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return { catCount: 0 };
  },
  methods: {
    addCat() {
      this.$emit("addCats");
    },
  },
};
</script>
