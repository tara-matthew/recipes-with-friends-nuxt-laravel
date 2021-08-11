<template>
    <div class="grid w-100 grid-cols-2 grid-rows-2 h-screen">
        <div v-for="(card, index) in homeCards" :key="index">
            <home-card :cardItems="card.items" :title="card.title"></home-card>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api';
import HomeCard from '~/components/molecules/HomeCard/HomeCard.vue';

export default defineComponent({
    components: { HomeCard },
    props: {
        homeCards: {}
    }
});

</script>
