<template>
  <section>
    <div class="grid grid-rows-2 grid-flow-col gap-4 m-2 bg-slate-400">
      <div class="bg-red-700 grid grid-cols-2" v-for="(item, i) in arr1">
        <span class="col-span-1 bg-blue-300 text-white-300">{{ arr1[i] }}</span>
        <span class="col-span-1 bg-blue-300 text-white-300">{{ arr2[i] }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'gridbrik',
  data: () => {
    return {
      // r1: this.arrsObj['arr1'],
      // r2: this.arrsObj['arr2'],
    };
  },
  props: {
    arrsObj: {
      type: Object,
      required: true,
    },
  },
  computed: {
    arr1() {
      return this.arrsObj['arr1'];
    },
    arr2() {
      return this.arrsObj['arr2'];
    },
  },
};
</script>

<style></style>
