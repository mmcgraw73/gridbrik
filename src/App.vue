<template>
  <main class="min-h-screen bg-gray-100 p-12">
    <h1 class="text-3xl font-bold mb-8">gridbrik</h1>
    <gridbrik :arrsObj="arrsObj" />
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
      arrsObj: {
        arr1: ['1', '2', '3', '4', '5', '6', '7', '8', '9'],
        arr2: [
          'one',
          'two',
          'three',
          'four',
          'five',
          'six',
          'seven',
          'eight',
          'niner',
        ],
      },
    };
  },
};
</script>
