<script setup>
import DraverHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed right-0 top-0 z-20 p-8">
    <DraverHead />
    <CartItemList />
    <div class="flex flex-col gap-4 mt-7">
      <div class="flex gap-2 items-end">
        <span>Total:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>1205 ₽</b>
      </div>
      <div class="flex gap-2 items-end">
        <span>Tax:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>60 ₽</b>
      </div>
      <button
        disabled=""
        class=" mt-4 transition bg-lime-500 w-full rounded-xl py-3 disabled:bg-slate-400 text-white hover:bg-lime-600 active:bg-lime-700 cursor-pointer"
        >
          Checkout
      </button>
    </div>
    
  </div>
</template>
