<template>
    <f7-page>
        <f7-navbar title="Zar Atma"></f7-navbar>
        <!--<div :class="'dice dice-' + diceOne "></div>-->
        <!--<div :class="'dice dice-' + diceTwo "></div>-->



        <div class="wrapper">
            <div id="alpha" class="die">
                <span class="a two three four five six"></span>
                <span class="b four five six"></span>
                <span class="c six"></span>
                <span class="d one three five"></span>
                <span class="e six"></span>
                <span class="f four five six"></span>
                <span class="g two three four five six"></span>
            </div>
            <div id="bravo" class="die">
                <span class="a two three four five six"></span>
                <span class="b four five six"></span>
                <span class="c six"></span>
                <span class="d one three five"></span>
                <span class="e six"></span>
                <span class="f four five six"></span>
                <span class="g two three four five six"></span>
            </div>

            <f7-button class="button-dice" fill color="blue" @click="random">Zar At</f7-button>
        </div>
    </f7-page>

</template>
<script>
    import $ from 'jquery'
export default {

    data() {
        return {
            diceOne: 6,
            diceTwo: 6
        }
    },
    created() {

    },
    methods: {
        random() {
            const self = this;
            self.diceOne = Math.floor(Math.random() * 6) + 1;
            self.diceTwo = Math.floor(Math.random() * 6) + 1;
        },
    }
};

</script>

<style lang="scss">
    /*
 * Dice.css v1.0
 * Code - MIT License - https://github.com/diafygi/dice-css
 * Images - Public Domain - https://openclipart.org/detail/105931/sixsided-dice-faces-lio-01
 */
    /*.dice-custom-1 {*/
        /*width: 70px;*/
        /*height: 70px;*/
        /*background-color: red;*/
        /*padding: 7px;*/
        /*border-radius: 3px;*/
        /*span {*/
            /*display: flex;*/
            /*align-items: center;*/
            /*justify-content: center;*/
            /*width: 10px;*/
            /*height: 10px;*/
            /*border-radius: 50%;*/
            /*background-color: #fff;*/
        /*}*/
    /*}*/
    /*.dice {*/
        /*display: inline-block;*/
        /*min-height: 5em;*/
        /*padding-left: 5em;*/
        /*background-size: 5em;*/
        /*background-repeat: no-repeat;*/

    /*}*/

    /*.dice-1 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cg transform='translate(113.25%2C-494.1)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-406.5%2C374.7)'%3E%3Crect x='588' y='240.4' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(337.5%2C87.5)' cx='325' cy='227.4' r='12.5' style='fill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E ");*/
    /*}*/

    /*.dice-2 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cstyle%3E.s0%7Bfill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000%3B%7D%3C%2Fstyle%3E%3Cg transform='translate(109.9%2C-505.1)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-415.6%2C485.6)'%3E%3Crect x='613' y='40.4' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(326.5%2C-148.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(398.5%2C-76.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E ");*/
    /*}*/

    /*.dice-3 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cstyle%3E.s0%7Bfill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000%3B%7D%3C%2Fstyle%3E%3Cg transform='translate(84.9%2C-515.5)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-290.6%2C514.9)'%3E%3Crect x='413' y='2.9' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(126.5%2C-186)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(198.5%2C-114)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(162.5%2C-150)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E ");*/
    /*}*/

    /*.dice-4 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cstyle%3E.s0%7Bfill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000%3B%7D%3C%2Fstyle%3E%3Cg transform='translate(90.7%2C-499.7)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-302.7%2C367.8)'%3E%3Crect x='425.5' y='265.4' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(139%2C76.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(139%2C148.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(211%2C76.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(211%2C148.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E ");*/
    /*}*/

    /*.dice-5 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cstyle%3E.s0%7Bfill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000%3B%7D%3C%2Fstyle%3E%3Cg transform='translate(89.2%2C-510.5)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-194.9%2C372.3)'%3E%3Crect x='213' y='277.9' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(-73.5%2C89)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-73.5%2C161)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-1.5%2C89)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-1.5%2C161)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-37.5%2C125)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E ");*/
    /*}*/

    /*.dice-6 {*/
        /*background-image: url("data:image/svg+xml,%3Csvg xmlns='http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg' version='1.1' viewBox='0 0 76.5 76.5' height='21.6' width='21.6'%3E%3Cstyle%3E.s0%7Bfill%3A%23000%3Bstroke-width%3A3%3Bstroke%3A%23000%3B%7D%3C%2Fstyle%3E%3Cg transform='translate(86.2%2C-500.6)'%3E%3Cg transform='matrix(0.5%2C0%2C0%2C0.5%2C-98.2%2C356.2)'%3E%3Crect x='25.5' y='290.4' width='150' height='150' ry='50' rx='50' style='fill%3A%23fff%3Bstroke-width%3A3%3Bstroke%3A%23000'%2F%3E%3Ccircle transform='translate(-261%2C101.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-261%2C173.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-261%2C137.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-189%2C101.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-189%2C173.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3Ccircle transform='translate(-189%2C137.5)' cx='325' cy='227.4' r='12.5' class='s0'%2F%3E%3C%2Fg%3E%3C%2Fg%3E%3C%2Fsvg%3E");*/
    /*}*/

    * { box-sizing: border-box; }

    html, body {
        height: 100%;
        width: 100%;
        background:#eff3fa;
        font-family: sans-serif;
    }

    body {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .wrapper {
        text-align:center;
    }

    .die {
        height:100px;
        width: 100px;
        margin: 0 auto;
        margin-bottom: 1rem;
        background: #fff;
        position: relative;
        border-radius: 4px;
        border: 1px solid #ebebeb;
        border-right-width: 2px;
        border-left-width: 2px;
        border-bottom: 3px solid #ccc;
    }

    .die > span {
        height: 15px;
        width: 15px;
        background: #222;
        border-radius: 50px;
        position: absolute;
    }

    .die .a { top:15px;left:15px; }
    .die .b { top:15px;right: 15px; }
    .die .c { left: 15px;top: 40px; }
    .die .d { top: 40px;left:42px; }
    .die .e { top: 40px;right: 15px; }
    .die .f { bottom: 15px;left: 15px; }
    .die .g { bottom: 15px;right: 15px; }
    .die > span { opacity: 0; }



    .button-dice {
        position: fixed;
        bottom: 0;
        width: 100%;
        border-radius: 0 !important;
    }

    .hidden {
        visibility: hidden;
    }


</style>
