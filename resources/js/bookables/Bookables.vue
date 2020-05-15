<template>
    <div>
        <bookable-list-item item-title="Cheap Villa" item-content="A very cheap villa" :price="1000"/>
        <bookable-list-item item-title="Cheap Villa2" item-content="A very cheap villa2" :price="1500"/>
    </div>
</template>

<script>
    import BookableListItem from "./BookableListItem";
    export default {
        components: {
            BookableListItem
        },
        // beforeCreate() {
        //     console.log('before create');
        // },
        created() {
            console.log('create');
        },
        // beforeMount() {
        //     console.log('before mount');
        // },
        // mounted() {
        //     console.log('mount');
        // },
        // beforeDestroy() {
        //     console.log('before destroy');
        // },
        // destroyed() {
        //     console.log('destroy');
        // }
    }
</script>
