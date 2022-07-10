<template>
  <section class="footer">
    <div class="container">
      <div>
        <button class="btn-success" @click="++likes">
          <i class="fa fa-thumbs-up" aria-hidden="true">Like</i>
        </button>
        <button class="btn-danger" @click="++dislikes">
          <i class="fa fa-thumbs-down" aria-hidden="true">Dislike</i>
        </button>
      </div>
      <p class="d-flex align-items-center text-break">
      <div class="text-white">{{ likesPercentage.toFixed(2) }}% - {{ dislikePercentage.toFixed(2) }}%
      </div>
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "PageViews",
  data() {
    return {
      likes: 0,
      dislikes: 0,
    };
  },
  computed: {
    likesPercentage() {
      if (this.likes + this.dislikes === 0) return 0;
      return (this.likes * 100) / (this.likes + this.dislikes);
    },
    dislikePercentage() {
      if (this.likes + this.dislikes === 0) return 0;
      return (this.dislikes * 100) / (this.likes + this.dislikes);
    },
  },
  watch: {},
};
</script>

<style scoped>

</style>