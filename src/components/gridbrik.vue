<template>
  <section class="w-full">
    <div :class="['bg-slate-400']">
      <div class="grid grid-cols-7 gap-4" v-for="(item, i) in arr1">
        <span class="col-span-4 bg-blue-800 text-red-300 p-3 rounded-lg mb-2">{{
          arr1[i]
        }}</span>
        <span class="col-span-3 bg-blue-800 text-red-300 p-3 rounded-lg mb-2">{{
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
    longestArr() {
      let max = 0;
      let index = -1;
      this.arrsArr.forEach(function (a, i) {
        console.log(a);
        if (a.length > max) {
          max = a.length;

          index = i;
        }
        return max;
      });
    },
  },
};
</script>

<style></style>
