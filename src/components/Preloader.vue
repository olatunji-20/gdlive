<template>
  <div class="pre">
    <div class="sub"></div>
  </div>
</template>

<script>
export default {
  name: "Preloader",
  setup() {},
};
</script>

<style scoped>
.pre {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
}
.sub {
  border: 8px solid #cccccc;
  border-top: 8px solid #6B9B8F;
  width: 6rem;
  height: 6rem;
  border-radius: 50%;
  margin: 16rem auto;
  animation-name: spinner;
  animation-duration: 1.2s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
@keyframes spinner {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>