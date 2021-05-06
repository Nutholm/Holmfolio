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