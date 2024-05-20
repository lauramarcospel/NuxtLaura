<template>
    <div>
        <template>
    <div>
      <h1 class="text-3xl font-bold mx-10 my-10 text-orange-400">
      Welcome Home!
    </h1>
    <div class="grid grid-cols-4 gap-5 mx-10">
      <div v-for="p in products"></div>
      <NuxtLink :to="/products/$(p.id)">{{ p.title }}</NuxtLink>
    </div>
    </div>
  </template>
    </div>
</template>

<script setup>
 definePageMeta({
  layout: "products"
 })

const{data: products}= await useFetch('https://fakestoreapi.com/products')
</script>

