<template>
  <button
    @click="$emit('btn-click')"
    :style="{ background: color }"
    class="btn"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  },
  emits: ['btn-click'],
  // methods: {
  //   onClick() {
  //     console.log('Click');
  //   },
  // },
};
</script>
