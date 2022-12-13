<template>
    <div class="container">
        <h1>Soft Drinks</h1>
        <div class="cards">
            <div v-for="item in item" :key="item">
                <products :item="item"/>
            </div>
        </div>
    </div>
    <products/>
</template>

<script>
import products from '../components/Products.vue';

export default {
components: { 
    products
}    
}
</script>

<style scoped>

</style>