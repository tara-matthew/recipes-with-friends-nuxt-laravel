<template>
    <div class="border-b-2 border-black h-12 flex items-center justify-center">
        <h1>{{ title }}</h1>
    </div>
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
