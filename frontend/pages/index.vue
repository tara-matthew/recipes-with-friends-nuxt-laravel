<template>
    <home-card-grid :home-cards="homeCards" />
</template>

<script lang="ts">
import Vue from 'vue';
import HomeCardGrid from '~/components/organisms/HomeCardGrid/HomeCardGrid.vue';

export default Vue.extend({
    components: { HomeCardGrid },
    setup () {
        const homeCards: object = [
            {
                title: 'First card',
                items: [
                    'an item',
                    'another item'
                ]
            },
            {
                title: 'Second card',
                items: [
                    'second card item',
                    'another second card item'
                ]
            },
            {
                title: 'Third card',
                items: [
                    'third card item',
                    'another third card item'
                ]
            },
            {
                title: 'Fourth card',
                items: [
                    'fourth card item',
                    'another fourth card item'
                ]
            }
        ];

        return {
            homeCards
        };
    }
});
</script>
