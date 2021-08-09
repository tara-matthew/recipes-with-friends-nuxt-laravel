<template>
    <span>{{ title }}</span>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext, Data } from '@nuxtjs/composition-api';

export default defineComponent({
    props: {
        title: String
    },
    setup (props: Data) {
        onMounted(() => {
            console.log('here', props);
        });
    }
});

</script>
