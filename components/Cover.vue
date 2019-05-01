<template>
  <section>
    <div class="wrapperCover">

      <div>
        <img class="solipartyMapuche" src="~/assets/soliparty-logo1.png">
      </div>

      <div>
        <div class="cover" :style="{ backgroundImage: 'url(' + require(`@/assets/Mapuche_Webisite_Header_1080p.png`) + ')' }"></div>
      </div>

    </div>
  </section>
</template>

<script>

export default {

}


</script>

<style>

.solipartyMapuche {
  position: absolute;
  left: 50%;
  margin-left: -17.5em;
  margin-top: 2em;
  width: 35em;
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
  .solipartyMapuche {
    position: absolute;
    left: 50%;
    margin-left: -30%;
    margin-top: 2em;
    width: 60%;
  }
}

</style>
