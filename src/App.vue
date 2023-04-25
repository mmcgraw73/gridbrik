<template>
  <main class="min-h-screen bg-gray-100 p-12">
    <h1 class="text-3xl font-bold mb-8">gridbrik</h1>
    <gridbrik :arrsArr="arrsArr" />
  </main>
</template>

<script>
import gridbrik from './components/gridbrik.vue';
export default {
  name: 'App',
  components: {
    gridbrik,
  },
  data() {
    return {
      arrsArr: [
        [
          'Processing',
          'Staggered Out',
          'Capped',
          'Invalid Location',
          'Validation Error',
          'Processing Error',
          'Undefined Error',
        ],
        ['22882', '554', '33', '774', '882', '8', '993'],
      ],
    };
  },
};
</script>
