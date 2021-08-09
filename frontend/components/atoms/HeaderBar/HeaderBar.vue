<template>
    <h1>{{ title }}</h1>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext, Data } from '@nuxtjs/composition-api';

export default defineComponent({
    props: {
        title: String
    },
    setup (props: Data) {
        console.log(props.title);
    }
});

</script>
