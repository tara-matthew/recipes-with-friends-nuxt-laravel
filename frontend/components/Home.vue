<template>
    <h1 class="text-gray-700">Home</h1>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext } from '@nuxtjs/composition-api';

export default defineComponent({
    setup () {
        const { $axios }: any = useContext();
        async function fetchResults (): Promise<void> {
            await $axios.$get('/api/test');
        }

        onMounted(fetchResults);
    }
});

</script>
