<template>
  <div class="header-wrapper" id="headerId">
    <ul class="tabs">
      <li class="music" @click="$emit('open-music')">Music</li>
      <li class="video"><a href="#vidLinkId">Video</a></li>
      <li class="title">The Thumping Tommys</li>
      <li class="shows" @click="$emit('open-shows')">Shows</li>
      <li class="contact"><a href="#contactId">Contact</a></li>
    </ul>
  </div>
</template>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header-wrapper {
  position: absolute;
  width: 100%;
  display: flex;
  background-color: rgb(0, 0, 0, 0.01);
  color: antiquewhite;
}
.tabs {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
  margin: auto;
  padding: 0;
}
li {
  margin: 1rem;
}
li:hover:not(.title) {
  background-color: rgba(192, 184, 157, 0.5);
  border-radius: 4px;
  cursor: pointer;
}
.title {
  cursor: auto;
  font-size: 2rem;
}

a {
  text-decoration: none;
  color: antiquewhite;
}

@media screen and (max-width: 680px) {
  .tabs {
    min-width: 375px;
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    gap: 0px 0px;
    grid-template-areas:
      "music video shows contact"
      "title title title title";
  }
  .music {
    grid-area: music;
    margin-bottom: 0;
  }
  .video {
    grid-area: video;
    margin-bottom: 0;
  }
  .shows {
    grid-area: shows;
    margin-bottom: 0;
  }
  .contact {
    grid-area: contact;
    margin-bottom: 0;
  }
  .title {
    grid-area: title;
    margin-top: 0;
  }
}
</style>
