<template>
    <div>
        <header-bar title="Test" />
        <card-list-item title="an item" />
    </div>
</template>

<script lang="ts">
import { defineComponent, computed, ref, onMounted, onUpdated, onUnmounted, useContext } from '@nuxtjs/composition-api';
import HeaderBar from '~/components/atoms/HeaderBar/HeaderBar.vue';
import CardListItem from '~/components/atoms/CardListItem/CardListItem.vue';

export default defineComponent({
    components: { CardListItem, HeaderBar },
    props: {
        title: String
    },
    setup (props: Data) {
        console.log(props.title);
    }
});

</script>
