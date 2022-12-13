<template>
    <div class="products mb-4">
        <div class="card" v-for="{item, index} in products" :key="index">
            <img :src="item.image" class="card-img-top">
            <div class="card-body">
                <h6 class="card-title">{{item.name}}</h6>
                <p class="card-text">R{{item.price}}</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
products: [
    {
        id: 1,
        name: 'Fanta',
        image: 'https://www.fanta.com/content/dam/nagbrands/us/fanta/en/home/wtfanta/fanta-rainbow.png',
        price: 25

},
    {
        id: 2,
        name: 'Coca-Cola',
        image: 'https://www.fanta.com/content/dam/nagbrands/us/fanta/en/home/wtfanta/fanta-rainbow.png',
        price: 30

},
    {
        id: 3,
        name: 'Sprite',
        image: 'https://www.fanta.com/content/dam/nagbrands/us/fanta/en/home/wtfanta/fanta-rainbow.png',
        price: 20

},
    {
        id: 4,
        name: 'Stoney',
        image: 'https://www.fanta.com/content/dam/nagbrands/us/fanta/en/home/wtfanta/fanta-rainbow.png',
        price: 25

}
]
            }
        }
        
    }
</script>

<style scoped>


</style>