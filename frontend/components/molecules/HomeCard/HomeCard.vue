<template>
    <div>
        <div class="border-b-2 border-black h-12 flex items-center justify-center">
            <header-bar :title="title" />
        </div>
        <ul>
            <li v-for="item in cardItems" :key="item.title">
                <card-list-item :title="item"></card-list-item>
            </li>
        </ul>
    </div>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext, Data } from '@nuxtjs/composition-api';
import HeaderBar from '~/components/atoms/HeaderBar/HeaderBar.vue';
import CardListItem from '~/components/atoms/CardListItem/CardListItem.vue';

export default defineComponent({
    components: { CardListItem, HeaderBar },
    props: {
        cardItems: {},
        title: null
    },
    setup (props: Data) {
        onMounted(() => {
            console.log('here', props.cardItems);
        });
    }
});

</script>
