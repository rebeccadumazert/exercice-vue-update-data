<template>
  <div>
    <button @click="changeColor">cliiick on me</button>
    <div :style="{'background-color' : color}">HEYYYYYY</div>
  </div>
</template>

<script>
const COLORS = ["yellow", "red", "orange", "black"];
export default {
  name: "changeOnClick",
  data: () => ({
    color: "pink",
    index: 0
  }),
  methods: {
    changeColor() {
      this.intervalID = setInterval(() => {
        this.index = (this.index + 1) % COLORS.length;
        this.color = COLORS[this.index];
      }, 200);
    }
  }
};
</script>