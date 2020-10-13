<template>
  <main>
    <slot></slot>
    <div class="container"></div>
  </main>
</template>

<style scoped>
main {
  height: 150vh;
}
.container {
  height: 150vh;
  max-width: 680px;
  margin-left: auto;
  margin-right: auto;
  background-image: url("../assets/tommys-homepage-img.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
@media screen and (max-width: 500px) {
  .container {
    width: 100vw;
    background-size: 180%;
    background-position: 40% 0%;
  }
  .main {
    width: 100px;
    
  }
}
</style>