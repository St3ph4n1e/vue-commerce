<script setup lang="ts">
import type { ProductInterface } from '@/interfaces/product.interface';
import CartProduct from './CartProduct.vue';

defineProps<{
  cart: ProductInterface[]
}>()
</script>

<template>
  <div class="d-flex flex-column">
    <CartProduct v-for="product in cart" :product="product"/>
    
  </div>
</template>

<style lang="scss" scoped></style>