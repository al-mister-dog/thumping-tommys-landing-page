<template>
  <img src="../assets/banjo.png" alt="" />
  <div class="festival-info">
    <h2 class="title">Cropredy 2021</h2>
    <p class="message">{{ message }}</p>
    <p class="link">
      <a :href="link">Buy tickets here</a>
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message:
        "Tickets for Cropredy 2021 are back on sale! If you have already purchased tickets for 2020, these will be valid for 2021. They are barcoded so you don't need to do anything.",
      link: "https://fairportconvention.com/tickets",
    };
  },
};
</script>

<style scoped>
.festival-info {
  position: relative;
  max-width: 684px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  background-color: rgb(0, 0, 0, 0.01);
  color: antiquewhite;
  margin: auto;
  margin-bottom: 1.5rem;
}

.title {
  margin: 0;
}

.message {
  margin: 0;
}

.link {
  margin: 0;
  padding: 0.2rem;
}

.link a {
  text-decoration: none;
  color: white;
}
.link a:hover {
  background-color: rgba(192, 184, 157, 0.5);
  border-radius: 4px;
  cursor: pointer;
}
img {
  width: 70%;
  padding: 5rem 0;
  max-width: 500px;
}
</style>