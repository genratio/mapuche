<template>
  <section>
    <div class="wrapperCover">



      <div>
        <img class="djListe" src="~/assets/DJ_Liste_st.png">
      </div>



      <div>
        <div class="cover" :style="{ backgroundImage: 'url(' + require(`@/assets/Soli_background.png`) + ')' }"></div>
      </div>

    </div>
  </section>
</template>

<script>

export default {

}

</script>

<style>

.djListe {
  position: absolute;
  left: 50%;
  margin-left: -22.5em;
  margin-top: 2em;
  width: 45em;
}

.cover {
  max-width: 100%;
  min-height: 100vh;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: center top;
}

.cover h1 {
  color: #183613;
  padding-top: 1em;
  padding-left: 7.5em;
  font-size: 50px;
  font-weight: 500;
}
@media screen and (min-width: 1600px) {

}
@media screen and (max-width: 880px) {
  .wrapperCover {
    max-width: 100%;
    min-height: 100vh;
  }
  .cover {
    max-width: 100%;
    min-height: 100vh;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    background-position: center top;
  }
  .djListe {
    position: absolute;
    left: 50%;
    margin-left: -35%;
    margin-top: 4em;
    width: 70%;
  }
}

</style>
