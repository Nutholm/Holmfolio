<template>
  <div class="homepage">
    <div class="flex" id="About">
      <div class="MitFoto">
        <img src="../assets/Ikkemig.jpg" alt="" />
      </div>

      <div class="AboutText">
        <div>
          <h1>Welcome to my portfolio</h1>
          <p>
            Greetings, to formerly present myself, my name is something
            something
          </p>
        </div>
      </div>
    </div>

    <div class="Projects">Projects</div>

    <div id="slideshow">
      <v-carousel
        cycle
        height="400"
        hide-delimiter-background
        show-arrows-on-hover
      >
        <v-carousel-item v-for="(slide, i) in slides" :key="i">
          <v-sheet :color="colors[i]" height="100%">
            <v-row class="fill-height" align="center" justify="center">
              <div class="display-3">{{ slide }} Slide</div>
            </v-row>
          </v-sheet>
        </v-carousel-item>
      </v-carousel>
    </div>

    <div class="Cinema">
      Cinema

      <div class="Video1">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/Ho4e1fCkjB0"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>

      <div class="Video2">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/CssOKCwT9Qo"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
      slides: ["First", "Second", "Third", "Fourth", "Fifth"],
    };
  },
};
</script>

<style lang="scss">
@import "./src/styles/variables.scss";

.home {
  height: 200vh;
}

.flex {
  display: flex;
  justify-content: space-around;
}

.Video1 {
  overflow: hidden;
  /* 16:9 aspect ratio */
  padding-top: 56.25%;
  position: relative;
}

.Video1 iframe {
  border: 0;
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}

.Video2 {
  overflow: hidden;
  /* 16:9 aspect ratio */
  padding-top: 56.25%;
  position: relative;
}

.Video2 iframe {
  border: 0;
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
</style>