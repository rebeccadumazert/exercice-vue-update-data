<template>
  <div>
    <button @click="changeColor('red')">RED</button>
    <button @click="changeColor('yellow')">YELLOW</button>
    <button @click="changeColor('blue')">BLUE</button>
    <div :style="{'background-color' : color}">COUCOUUUUUU LE MONDE</div>
  </div>
</template>

<script>
export default {
  name: "clickclick",
  data: () => ({
    color: "white"
  }),
  methods: {
    changeColor(newColor) {
      this.color = newColor;
    }
  }
};
</script>