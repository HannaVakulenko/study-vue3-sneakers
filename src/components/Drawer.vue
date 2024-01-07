<script setup>
import DrawerHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8 flex flex-col justify-between">
    <DrawerHead />

    <CartItemList />

    <div class="flex flex-col gap-4 mt-7">
      <div class="flex gap-2 place-items-baseline">
        <span>Total:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>12990 UAH</b>
      </div>
      <div class="flex gap-2 place-items-baseline">
        <span>Tax 5%:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>650 UAH</b>
      </div>
      <button
        disabled=""
        class="mt-4 transition bg-lime-500 w-full rounded-xl py-3 text-white disabled:bg-slate-300 hover:bg-lime-600 hover:bg-lime-700 cursor-pointer"
      >
        Order
      </button>
    </div>
  </div>
</template>
