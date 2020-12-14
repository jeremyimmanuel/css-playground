<template>
    <div class="card">

    </div>
</template>

<script>
    export default {
        name: 'CardFour',

        data () {
            return {}
        }
    }
</script>

<style lang="scss" scoped>
.card {
    background: white;
    margin: 20px;
    padding: 20px 15px;
    border-radius: 8px;
    width: 250px;
    height: 250px;
    transition: 0.5s ease-in-out;
}

.card:hover {
    width: 500px;
    height: 500px;
    background: red;
}
</style>