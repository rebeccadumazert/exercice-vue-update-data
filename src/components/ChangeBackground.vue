<template>
  <div :style="{'background-color' : color}">hellooooo</div>
</template>

<script>
const COLORS = ["blue", "pink", "purple", "green"];
export default {
  name: "changeBackgroung",
  data: () => ({
    color: "blue",
    index: 0
  }),
  methods: {
    updateBackground() {
      this.intervalID = setInterval(() => {
        this.index = (this.index + 1) % COLORS.length;
        this.color = COLORS[this.index];
      }, 200);
    }
  },
  created() {
    return this.updateBackground();
  }
};
</script>

<style modul>
</style>