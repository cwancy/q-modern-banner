<template>
  <q-banner :class="`q-ma-lg base ${props.type}`">
    <div class="row items-center">
      <div class="q-mr-sm">
        <q-icon :name="props.icon" size="md" />
      </div>
      <div class="col">
        <div class="poppins-semibold q-mb-xs" style="font-size: large">
          {{ props.title }}
        </div>
        <div class="poppins-light">
          {{ props.subtitle }}
        </div>
      </div>
    </div>
  </q-banner>
</template>

<script setup>
import { onMounted } from 'vue'

const props = defineProps({
  type: {
    type: String,
    required: true,
  },
  icon: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  subtitle: {
    type: String,
    required: true,
  },
})

onMounted(() => {
  if (props.type === undefined) throw new Error('Missing type for Banner prop')
})
</script>

<style scoped>
.base {
  border-radius: 4px;
}
.error {
  background-color: #fdecea;
  color: #e74c3c;
  border: 1px solid #e74c3c;
}

.info {
  background-color: #e0f7fa;
  color: #00796b;
  border: 1px solid #00796b;
}

.success {
  background-color: #e6f9eb;
  color: #28a745;
  border: 1px solid #28a745;
}

.warn {
  background-color: #fff3e0;
  color: #f57c00;
  border: 1px solid #f57c00;
}
</style>
