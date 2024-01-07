<script setup>
import Card from './Card.vue'

const onClickAdd = () => {
  alert('Add')
}
</script>

<template>
  <div class="grid md:grid-cols-2 xl:grid-cols-4 gap-5">
    <Card
      title="Men's sneakers Nike Blaser Mid Suede"
      imageUrl="/sneakers/sneakers-1.jpg"
      :price="5000"
      :isFavorite="true"
      :onClickAdd="onClickAdd"
    />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
  </div>
</template>
