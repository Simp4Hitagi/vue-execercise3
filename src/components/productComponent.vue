<template>
    <div>
        <div v-if="productsArray.length">
            <div v-for="product in products" :key="product">
                <div class="card" style="width: 18rem;">
                    <img src="..." class="card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">{{ product.id }}</h5>
                      <p class="card-text">{{product.productName}}</p>
                      <p class="card-text">{{product.age}}</p>
                      
                    </div>
                </div>
            </div>
        </div>
        <!-- <div v-else>
            <spinner/>
        </div> -->
    </div>
</template>
<script>
import spinner from '@/components/Spinner.vue'
export default {
    name: 'products',
    components: {
        spinner
    },
    data(){
        return{
            productsArray: [
                {
                    id: 1,
                    productName: "Luntu",
                    age: "Appropriate"
                }
            ]   
        }
    }
    
}
</script>
<style scoped>
    
</style>