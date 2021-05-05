<template>
  <div class="flex" id="header">


    <div class="flex" id="UX1">
      <div>Home</div>
      <div>About</div>
    </div>

    <div id="Logo">
      <img src="../assets/micholas.png" alt="">
    </div>

    <div class="flex" id="UX2">
      <div>Projects</div>
      <div>Cinema</div>
    </div>


  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import '../styles/variables.scss';

.flex {
  display: flex;
  justify-content: space-around;
}

#header {
  
  width: 100%;
  height: 120px;
  background-color: map-get($Colorscheme, Primary);
}

#UX1, #UX2 {
  width: 25%;
  margin-top: 5%;
}


</style>