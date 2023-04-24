<template>
  <section>
    <div class="grid grid-rows-2 grid-flow-col gap-4 m-2 bg-slate-400">
      <div class="bg-red-700 grid grid-cols-2" v-for="(item, i) in r1">
        <span class="col-span-1 bg-blue-300 text-white-300">{{ r1[i] }}</span>
        <span class="col-span-1 bg-blue-300 text-white-300">{{ r2[i] }}</span>
      </div>
      <!-- <div class="bg-red-700">02</div>
      <div class="bg-red-700">03</div>
      <div class="bg-red-700">04</div>
      <div class="bg-red-700">05</div>
      <div class="bg-red-700">06</div>
      <div class="bg-red-700">07</div>
      <div class="bg-red-700">08</div>
      <div class="bg-red-700">09</div> -->
    </div>
  </section>
</template>

<script>
const repeater1 = ['1', '2', '3', '4', '5', '6', '7', '8', '9'];
const repeater2 = [
  'one',
  'two',
  'three',
  'four',
  'five',
  'six',
  'seven',
  'eight',
  'niner',
];
export default {
  name: 'gridbrik',
  data: () => {
    return {
      r1: repeater1,
      r2: repeater2,
    };
  },
};
</script>

<style></style>
