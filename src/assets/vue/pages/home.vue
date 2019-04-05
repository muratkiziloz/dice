<template>
    <f7-page>
        <div class="container">
            <div :class="'fi dice-icon-' + diceOne"></div>
            <div :class="'fi dice-icon-' + diceTwo"></div>
            <button class="button-dice" @click="random">ZAR AT</button>
        </div>
    </f7-page>

</template>
<script>
    import $ from 'jquery'
export default {

    data() {
        return {
            diceOne: 6,
            diceTwo: 6,
        }
    },
    created() {

    },
    methods: {
        random() {
            const self = this;
            setTimeout(function () {
                self.diceOne = Math.floor(Math.random() * 6) + 1;
                self.diceTwo = Math.floor(Math.random() * 6) + 1;
            },1000);

            $('.fi').addClass('active');
            setTimeout(function () {
                $('.fi').removeClass('active');

            },500)

        }
    }
};

</script>
