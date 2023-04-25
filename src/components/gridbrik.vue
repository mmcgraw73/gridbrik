<template>
  <section class="w-full">
    <div :class="['bg-slate-400 p-2']">
      <div class="grid grid-cols-7 gap-4 m-2" v-for="(item, i) in arr1">
        <span class="col-span-3 bg-blue-800 text-red-300 p-3 rounded-lg mb-2">{{
          arr1[i]
        }}</span>
        <span class="col-span-4 bg-blue-800 text-red-300 p-3 rounded-lg mb-2">{{
          arr2[i]
        }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'gridbrik',
  props: {
    arrsArr: {
      type: Array,
      required: true,
    },
  },
  computed: {
    arr1() {
      return this.arrsArr[0];
    },
    arr2() {
      return this.arrsArr[1];
    },
  },
};
</script>

<style></style>
