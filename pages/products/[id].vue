<template>
    <div>
        <template>
    <div>
      <h1 class="text-3xl font-bold mx-10 my-10 text-orange-400">
      Catalogo
    </h1>
    <p> Detalle del articulo {{ id }}</p>
    </div>
  </template>
    </div>
</template>

<script setup>
 const { id } = useRoute().params
</script>
