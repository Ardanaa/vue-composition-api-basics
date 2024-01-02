<template>
  <div class="w-full">
    <div class="flex gap-2 items-center justify-center">
      <v-btn @click="decraseCounter" class="text">-</v-btn>
      <span class="text-xl">{{ counter }}</span>
      <v-btn @click="increaseCounter" class="text">+</v-btn>
    </div>
  </div>
</template>


<!-- Composition API -->
<script setup>
import { ref } from 'vue'

const counter = ref(0)
    
    const increaseCounter = () => {
      counter.value++
    }
    const decraseCounter = () => {
      counter.value--
    }
</script>

<!-- <script>
import { ref } from 'vue'

export default {
  setup() {
    const counter = ref(0)
    
    const increaseCounter = () => {
      counter.value++
    }
    const decraseCounter = () => {
      counter.value--
    }

    return {
      counter,
      increaseCounter,
      decraseCounter
    }
  }
}
</script> -->


<!-- Options API -->
<!-- <script>
export default {
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increaseCounter() {
      this.counter++
    },
    decraseCounter() {
      this.counter--
    }
  }
}
</script> -->