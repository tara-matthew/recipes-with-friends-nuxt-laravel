<template>
    <h1>Home</h1>
</template>

<script lang="ts">
export default {
  mounted() {
    console.log('mounted');
    this.fetchResults();
  },
  methods: {
    async fetchResults() {
      let res = await this.$axios.$get('/api/test')
      console.log(res);
    }
  }
}

</script>
