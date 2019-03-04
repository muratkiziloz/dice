<template>
    <f7-page>
        <f7-navbar title="Zar Atma"></f7-navbar>
        <img :src="image" alt="">
        <f7-button fill color="blue">Blue</f7-button>

    </f7-page>
</template>
<script>
    import $ from 'jquery'
export default {

    data() {
        return {
            one: 1,
            two: 2,
            three: 3,
            four: 4,
            five: 5,
            six: 6,
            image: './static/images/1.png/',
        }
    },
    created() {

    },
    methods: {
        random() {

            document.getElementById("demo").innerHTML = Math.floor(Math.random() * 10);
        }
    }
};

</script>
