<template>
    <h1>Home</h1>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext } from '@nuxtjs/composition-api';

export default defineComponent({
  setup () {
    const { $axios }: any = useContext()
    async function fetchResults (): Promise<void> {
      const res: any = await $axios.$get('/api/test')
      console.log(res)
    }
    onMounted(fetchResults)
  }
})

</script>
