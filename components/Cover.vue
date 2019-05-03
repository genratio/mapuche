<template>
  <section>
    <div class="wrapperCover">

      <div>
        <div class="cover" :style="{ backgroundImage: 'url(' + require(`@/assets/Mapuche_Webisite_Header_1080p.png`) + ')' }">
          <img class="djListe" src="~/assets/soliparty-logo1.png">
        </div>
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
  display: block;
  margin-left: auto;
  margin-right: auto;
  padding-top: 2em;
  padding-bottom: 2em;
  width: 50%;
  max-height: 100%;
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
  .solipartyMapucheText {
    position: absolute;
    left: 50%;
    padding-top: 2em;
    padding-bottom: 2em;
    margin-left: -45%;
    margin-top: 2em;
    width: 90%;
  }
}
/* If height very low */
@media screen and (max-height: 500px) {
  .solipartyMapucheText {
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding-top: 2em;
    padding-bottom: 2em;
    width: 90%;
    max-height: 100%;
  }
}

</style>
