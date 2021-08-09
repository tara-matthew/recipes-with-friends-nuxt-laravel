<template>
    <div>
        <div v-for="(card, index) in homeCards" :key="index">
            <home-card :cardItems="card.items" :title="card.title"></home-card>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent, onMounted } from '@nuxtjs/composition-api';
import HomeCard from '~/components/molecules/HomeCard/HomeCard.vue';

export default defineComponent({
    components: { HomeCard },
    props: {
        homeCards: {}
    },
    setup (props: Data) {
    }
});

</script>
