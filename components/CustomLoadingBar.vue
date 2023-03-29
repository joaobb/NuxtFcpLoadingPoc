<template>
  <div>
    <div id="custom-loading-bar" style="background: red; height: 20px"></div>
  </div>
</template>

<style scoped>
@keyframes barGrow {
  from {
    right: 100%;
  }
  to {
    right: 0;
  }
}

#custom-loading-bar {
  position: fixed;
  top: 0;
  left: 0;

  animation: barGrow 5s ease-in-out;
}
</style>
