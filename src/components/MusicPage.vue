<template>
  <div class="music-wrapper">
    <h2 class="music-h2">
      <a
        href="https://thethumpingtommys.bigcartel.com/products?page=2/"
        target="_blank"
        >Buy</a
      >
    </h2>
    <h2 class="music-h2">
      <a
        href="https://open.spotify.com/artist/4I0IGVeYiw9eS3NcehE1ge"
        target="_blank"
        >Listen</a
      >
    </h2>
    <h2 class="music-h2">
      <a
        href="https://www.youtube.com/channel/UChZo1tTCzlVYIiM3rS34eSQ"
        target="_blank"
        >Watch</a
      >
    </h2>
    <p class="music-p" @click="$emit('close-music')">close</p>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.music-wrapper {
  height: 100vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: black;
  color: antiquewhite;
}

.music-h2 {
  padding: 0.4rem;
}

.music-p {
  padding: 0.4rem;
}
.music-h2:hover,
.music-p:hover {
  cursor: pointer;
  border-radius: 4px;
  background-color: rgba(192, 184, 157, 0.5);
  padding: 0.4rem;
}

a {
  text-decoration: none;
  color: antiquewhite;
}
</style>