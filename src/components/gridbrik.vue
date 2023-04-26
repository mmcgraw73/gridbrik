<template>
  <section class="w-full">
    <div :class="['p-2']">
      <div class="grid grid-cols-10 gap-4 m-2" v-for="(item, i) in arr1">
        <span class="col-span-7 p-3 rounded-lg mb-2">{{ arr1[i] }}</span>
        <span
          :class="[
            'col-span-3 text-grey-200 text-white font-semibold p-3 rounded-full mb-2 text-center',
            i < 2 ? 'bg-green-600' : 'bg-red-400',
          ]"
          >{{ arr2[i] }}</span
        >
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
