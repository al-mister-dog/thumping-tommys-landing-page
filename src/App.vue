//TODO
// compile site for production

<template>
  <div id="app">
    <transition>
      <music-page
        @close-music="closeMusicPage"
        v-if="musicPageVisible === true"
      ></music-page>
    </transition>
    <transition>
      <shows-page
      @close-shows="closeShowsPage"
      v-if="showsPageVisible === true">
      </shows-page>
    </transition>
    <div v-if="musicPageVisible === false && showsPageVisible === false">
      <main-image> 
            <transition>
      <the-header
        @open-music="openMusicPage"
        @open-shows="openShowsPage"
        v-if="musicPageVisible === false && showsPageVisible === false"
      ></the-header>
    </transition>
      </main-image>
      <fest-info></fest-info>
      <fest-image></fest-image>
      <the-videos></the-videos>
      <the-bio></the-bio>
      <the-footer></the-footer>
    </div>
  </div>
</template>

<script>
import MainImage from "./components/MainImage.vue";
import FestInfo from "./components/FestInfo.vue";
import FestImage from "./components/FestImage.vue";
import TheVideos from "./components/TheVideos.vue";
import TheBio from "./components/TheBio.vue";
import TheFooter from "./components/TheFooter.vue";
import TheHeader from "./components/TheHeader.vue";
import MusicPage from "./components/MusicPage.vue";
import ShowsPage from "./components/ShowsPage.vue"

export default {
  name: "App",
  components: {
    MainImage,
    FestInfo,
    FestImage,
    TheVideos,
    TheBio,
    TheFooter,
    TheHeader,
    MusicPage,
    ShowsPage
  },
  data() {
    return {
      musicPageVisible: false,
      showsPageVisible: false,
    };
  },
  methods: {
    openMusicPage() {
      this.musicPageVisible = !this.musicPageVisible;
    },
    closeMusicPage() {
      this.musicPageVisible = !this.musicPageVisible;
    },
    openShowsPage() {
      this.showsPageVisible = !this.showsPageVisible;
    },
    closeShowsPage() {
      this.showsPageVisible = !this.showsPageVisible;
    },
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}
html {
  scroll-behavior: smooth;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
}

body {
  margin: 0;
  padding: 0;
  background-image: linear-gradient(
    to bottom,
    black 0,
    black 15%,
    #593e3d 50%,
    black 100%
  );
}

/* TRANSITIONS */

.v-enter-from {
  opacity: 0;
}
.v-enter-active {
  transition: all 1s ease-out;
}
.v-enter-to {
  opacity: 1;
}
.v-leave-from {
  opacity: 1;
}
.v-leave-active {
  transition: all 0.5s ease-out;
}
.v-leave-to {
  opacity: 0;
}

@media screen and (max-width: 414px) {
  html,body{
    overflow-x: hidden;
}
}
</style>
