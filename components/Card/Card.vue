<template>
  <div class="card w-96 bg-base-100 card-xs shadow-sm">
    <div class="card-body">
      <h2 class="card-title">
        <button class="flex justify-between items-center w-full" @click="$emit('click')">
          <span>{{ props.title }}</span>
            <Icon name="material-symbols:arrow-forward-ios-rounded" style="color: white" />
        </button>
      </h2>
      <div class="justify-end card-actions">
        
      </div>
    </div>
  </div>
</template>

<script setup>


const props = defineProps({
  title: {
    type: String,
    default: 'Card Title',
  },
})

const emit = defineEmits(['click'])

</script>