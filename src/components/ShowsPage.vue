<template>
  <div class="shows-wrapper">
    <h2 class="shows-h2">
      No upcoming shows
    </h2>
    <p class="shows-p" @click="$emit('close-shows')">close</p>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.shows-wrapper {
  height: 100vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: black;
  color: antiquewhite;
}

.shows-h2 {
  padding: 0.4rem;
}

.shows-p {
  padding: 0.4rem;
}

.shows-p:hover {
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