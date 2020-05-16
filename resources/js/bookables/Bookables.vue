<template>
    <div>
        <bookable-list-item v-if="bookable1" :item-title="bookable1.title" :item-content="bookable1.content" :price="1000"/>
        <bookable-list-item v-if="bookable2" :item-title="bookable2.title" :item-content="bookable2.content" :price="1500"/>
    </div>
</template>

<script>
    import BookableListItem from "./BookableListItem";
    export default {
        components: {
            BookableListItem
        },
        data() {
            return {
                bookable1: null,
                bookable2: null,
            }
        },
        // beforeCreate() {
        //     console.log('before create');
        // },


        created() {
            setTimeout(() => {
                this.bookable1 = {
                    title: "Cheap Villa",
                    content: "A very cheap villa",
                };
                this.bookable2 =  {
                    title: "Cheap Villa 2",
                    content: "A very cheap villa 2",
                };
            }, 2000);
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
