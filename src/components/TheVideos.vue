<template>
  <img src="../assets/violin.png" alt="" />
  <div class="video-wrapper" id="vidLinkId">
    <iframe
      class="video-frame"
      src="https://www.youtube.com/embed/L4wyJ8LlmYg"
    ></iframe>
    <iframe
      class="video-frame"
      src="https://www.youtube.com/embed/xkjiif9qcYc"
    ></iframe>
    <iframe
      class="video-frame"
      src="https://www.youtube.com/embed/pgTrUCB_hq4"
    ></iframe>
    <iframe
      class="video-frame"
      src="https://www.youtube.com/embed/bXoeV2ZETU8"
    ></iframe>
  </div>
</template>


<style scoped>
.video-wrapper {
  height: 200vh;
  width: 100%;
  display: flex;
  flex-direction: column;
}
.video-frame {
  width: 80vh;
  height: 50vh;
  margin: 2rem auto;
}
img {
  width: 70%;
  padding: 5rem 0;
  max-width: 500px;
}

@media screen and (max-width: 500px) {
  .video-frame {
  width: 100vw;
  height: 50vh;
  margin-top: 5px;
}
}
</style>


 
 
 
 