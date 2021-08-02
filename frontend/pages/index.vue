<template>
  <HomeCard />
</template>

<script lang="ts">
import Vue from 'vue'
import HeaderBar from '~/components/atoms/HeaderBar/HeaderBar.vue'
import HomeCard from "~/components/molecules/HomeCard/HomeCard.vue";

export default Vue.extend({
  components: {HomeCard, HeaderBar }
})
</script>
