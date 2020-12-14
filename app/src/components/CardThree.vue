<template>
    <button
        :disabled="disableButton"
        @click="() => show = !show"
    >
        Show
    </button>
    <transition name="bounce">
        <div
            v-if="show"
            class="card"
            @animationstart="onAnimationStart"
            @animationend="onAnimationEnd"
            @transitionend="onTransitionEnd"
        >
            Card
        </div>
    </transition>
</template>

<script>
export default {
    name: 'CardThree',

    data () {
        return {
            show: false,
            disableButton: false
        }
    },

    methods: {
        printHi () {
            console.log('hi')
        },
        onTransitionEnd () {
            console.log('onTransitionEnd')
        },
        onAnimationStart () {
            this.disableButton = true
            console.log('onAnimationStart')
        },
        onAnimationEnd () {
            this.disableButton = false
            console.log('onAnimationEnd')
        }
    }
}
</script>

<style lang="scss" scoped>
.card {
    background: white;
    margin: 20px;
    padding: 20px 15px;
    border-radius: 8px;
}

.bounce-enter-active {
    animation: bounce 0.5s ease-out both;
}

.bounce-leave-active {
    animation: bounce 0.5s reverse ease-in both;
}

@keyframes bounce {
    0% {
        transform: scale(0);
    }
    50% {
        transform: scale(1.25);
    }
    100% {
        transform: scale(1);
    }
}

button {
    position: absolute;
}

</style>