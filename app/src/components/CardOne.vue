<template>
    <div class="card">
        <div class="imgBox">
            <img :src="imgLink">
        </div>
        <div class="content">
            <h2>{{ title }}</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora aut deleniti dolorum natus tempore dolores! Quaerat minus dolores fugiat optio tempore ut in debitis voluptates quisquam! Nobis modi optio natus.</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardOne',

    props: {
        title: String,
        imgLink: String
    },

    data () {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
.card {
    position: relative;
    max-width: 300px;
    height: 215px;
    background: white;
    margin: 30px 30px;
    padding: 20px 15px;
    display: flex;
    flex-direction: column;
    // box-shadow: 0 5px 20px rgba(0, 0, 0, 0.5);
    transition: 0.5s ease-in-out;
}

.card:hover {
    height: 420px;
}

.imgBox {
    position: relative;
    width: 260px;
    height: 260px;
    top: -60px;
    left: 20px;
    z-index: 1;
    // box-shadow: 0 5px 202px rgba(0, 0, 0, 0.5);
}

img {
    max-width: 100%;
    border-radius: 8px;
}

.content {
    position: relative;
    margin-top: -140px;
    padding: 10px 15px;
    text-align: center;
    color: #111;
    visibility: hidden;
}

.card:hover .content{
    visibility: visible;
    opacity: 1;
    margin-top: -40px;
    transition-delay: 0.3x;
}
</style>