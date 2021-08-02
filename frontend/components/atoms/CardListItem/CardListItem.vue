<template>
    <span>{{ title }}</span>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext } from '@nuxtjs/composition-api';

export default defineComponent({
    props: {
        title: String
    },
    setup (props: Data) {
        console.log(props.title);
    }
});

</script>
