<template>
    <div
        class="card"
        @mouseover="() => showContent = true"
        @mouseleave="() => showContent = false"
    >
        <div class="top-header">
            <img :src="imgLink">
            <h1>{{ title }}</h1>
            <transition
                name="content-fade"
            >
                <p
                    v-show="showContent"
                    class="content"
                >
                    {{ lorem }}
                </p>
            </transition>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardTwo',

    data () {
        return {
            showContent: false,
            lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora aut deleniti dolorum natus tempore dolores! Quaerat minus dolores fugiat optio tempore ut in debitis voluptates quisquam! Nobis modi optio natus."
        }
    },

    props: {
        imgLink: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>
.content-fade-enter-active {
    transition: all .75s ease-out 0.1s;
}

.content-fade-leave-active {
    transition: all .5s cubic-bezier(1.0, .5, .8, 1) -.1s;
}

.content-fade-enter-from,
.content-fade-leave-to {
    opacity: 0;
    transform: translateY(-40px);
    // transform: scale(2, 0.5);
}

.content {
    width: 260px;
}

.card {
    display: flex;
    position: relative;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    background: white;
    padding: 20px 15px;
    border-radius: 8px;

    height: 175px;
    transition: all .8s ease-in-out;
}

.card:hover {
    height: 300px;
}

.top-header {
    position: absolute;
    top: -50px;
    width: 250px;
}

img {
    max-width: 100%;
    border-radius: 8px;
}
</style>