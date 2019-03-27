<template>
    <div class="product">
        <div class="product-detail">
        {{ product }}
        </div>

        <form @submit.prevent="submitProduct(product)">
            <input v-model="product" />
            <button type="submit">Submit</button>
        </form>
    </div>

</template>

<script>
    export default {
        name: "Product",
        data() {
            return {
                product: "Socks"
            }
        },
        methods: {
            submitProduct(product) {
                alert (product);
            }
       }
    }
</script>

<style scoped>

</style>