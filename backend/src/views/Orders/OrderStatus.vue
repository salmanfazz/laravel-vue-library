<template>
  <span class="text-white py-1 px-2 rounded " :class="{
      'bg-emerald-500': order.status === 'Kembali',
      'bg-orange-400': order.status === 'shipped',
      'bg-red-500': order.status === 'cancelled',
      'bg-gray-400': order.status === 'Pinjam',
    }">{{ order.status }}</span>
</template>

<script setup>
const {order} = defineProps({
  order: Object
})
</script>

<style scoped>

</style>
