<template>
  <div>
    <h1 class="text-lg mb-3">Subject Groups</h1>
    <div class="flex flex-col gap-4">
      <Card :title="Physics" @click="handleClick" />
      <Card :title="Chemistry" @click="handleClick" />
    </div>
  </div>
</template>

<script setup>

const handleClick = () => {
  console.log('Card clicked')
}


</script>