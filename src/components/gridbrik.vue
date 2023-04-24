<template>
  <section class="w-full">
    <div :class="['bg-slate-400', rowsClass]">
      <div class="grid grid-cols-7 gap-4" v-for="(item, i) in arr1">
        <span class="col-span-4 bg-blue-800 text-red-300 p-3 rounded-lg">{{
          arr1[i] || 'empty'
        }}</span>
        <span class="col-span-3 bg-blue-800 text-red-300 p-3 rounded-lg">{{
          arr2[i] || 'empty'
        }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'gridbrik',
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
    rowsClass() {
      return `grid grid-rows-${this.arr1.length} gap-3`;
    },
  },
};
</script>

<style></style>
