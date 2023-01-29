<template>
  <div>Welcome to watcher</div>
  <div>Counter {{ count }}</div>
  <button v-on:click="incCount()">+</button>
  <button v-on:click="decCount()">-</button>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Watcher",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    incCount() {
      console.log("click");
      this.count = this.count + 1;
    },
    decCount() {
      this.count = this.count - 1;
    },
  },
  watch: {
    count(newVal, prevVal) {
      alert(JSON.stringify({newVal, prevVal}));
    },
  },
};
</script>