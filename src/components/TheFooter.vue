<template>
  <link
    rel="stylesheet"
    href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
  />
  <img src="../assets/violin.png" alt="" />
  <div class="wrapper" id="contactId">
    <h2>Contact</h2>
    <p>{{ p1 }}</p>
    <p>{{ p2 }}</p>
    <ul>
      <li class="social">
        <a href="https://twitter.com/thumpingtommys"
        target="_blank"
        ><i class="fa fa-twitter"></i></a>
      </li>
      <li class="social">
        <a href="https://www.facebook.com/thethumpingtommys"
        target="_blank"
        ><i class="fa fa-facebook"></i></a>
      </li>
      <li class="social">
        <a href="https://open.spotify.com/artist/4I0IGVeYiw9eS3NcehE1ge"
        target="_blank"
        ><i class="fa fa-spotify"></i></a>
      </li>
      <li class="social">
        <a href="https://www.instagram.com/thethumpingtommys"
        target="_blank"
        ><i class="fa fa-instagram"></i></a>
      </li>
      <li class="social">
        <a href="https://www.youtube.com/channel/UChZo1tTCzlVYIiM3rS34eSQ"
        target="_blank"
        ><i class="fa fa-youtube"></i></a>
      </li>
    </ul>
    <h3><a href="#headerId">Home</a></h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      p1:
        "We play all sorts of events from pubs, clubs and festivals to weddings and business events.",
      p2: "Please send gig and event queries to thethumpingtommys@gmail.com",
    };
  },
};
</script>

<style scoped>
.wrapper {
  height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  color: antiquewhite;
}
ul {
  display: flex;
  list-style: none;
  justify-content: center;
  align-items: center;
  padding: 0;
}
.social {
  margin: 1rem;
}
img {
  width: 70%;
  padding: 5rem 0;
  max-width: 500px;
}
a {
  text-decoration: none;
  color: antiquewhite;
}

</style>