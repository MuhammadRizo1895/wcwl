<template>
  <div class="pagination">
    <button @click="previousPage" :disabled="currentPage === 1">
      Previous
    </button>
    <span>{{ currentPage }} / {{ totalPages }}</span>
    <button @click="nextPage" :disabled="currentPage === totalPages">
      Next
    </button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      currentPage: 1,
      itemsPerPage: 12,
      totalItems: this.CurrentImages.length,
    };
  },
  computed: {
    totalPages() {
      return Math.ceil(this.totalItems / this.itemsPerPage);
    },
  },
  methods: {
    previousPage() {
      if (this.currentPage > 1) {
        this.currentPage--;
      }
    },
    nextPage() {
      if (this.currentPage < this.totalPages) {
        this.currentPage++;
      }
    },
  },
};
</script>
<style></style>
