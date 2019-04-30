<template>
  <section class="pageWrapper">
    <section class="pageInnerWrapper">
      <img src="~/assets/soliankündigung.png" class="headerPic">
      <h2>Für <b>Juana Calfunao Paillalef</b> - Sie ist Lonco (Oberhaupt) einer Mapuche Community in Südchile.</h2>
      <h2 class="subHeadingInfobox">In diesem Video erzählt sie ihre Geschichte:</h2>

      <!--<p style="margin-top:1em;">
        Hier bekommt ihr einen Eindruck um wen es geht:
      </p>-->

      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/EGMSoZ6yvv4?&showinfo=0&rel=0" width="100%" height="auto" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="allowfullscreen"></iframe>
      </div>

      <div id="containerProfile">
        <img src="~/assets/JuanaMountainCubeRight.png" class="profile">
      </div>

      <p style="margin-top:3em;">
        <b>Juana Calfunao Paillalef</b> verklagt den chilenischen Staat vor dem lateinamerikanischen Gerichtshof für die Anerkennung der Menschenrechtsverletzungen gegenüber der Mapuche. Sie und ihre Familie haben wegen ihrer Rolle als Aktivistin und Lonco gewaltige Repressionen vom chilenischen Staat erfahren. Sie wurde ohne Prozess inhaftiert, gefoltert, ihr Haus wurde zwei Mal niedergebrannt und vieles mehr. Sie konnte an den Prozesstagen im Februar nicht anwesend sein, da sie nicht die Mittel für die Reisekosten aufbringen konnte. Daraufhin wurde ihr die Immunität temporär abgesprochen und somit befindet sie sich derzeit in großer Gefahr!
      </p>

      <div class="galleryContainer">
        <div>
          <img class="galleryImage" src="~/assets/JuanaPolice2.jpg">
        </div>
        <div>
          <img class="galleryImage" src="~/assets/JuanaDemo.jpg">
        </div>
        <div>
          <img class="galleryImage" src="~/assets/JuanaWounded2.jpg">
        </div>
      </div>

      <p style="margin-top:1em;">
        Wir vereinen uns gegen die Repressionen an einer Mapuche Community! Einen Staat vor dem Interamerikanischen Gerichtshof wegen Menschrenrechtsverbrechen zu verklagen ist sehr teuer! Wir unterstützen mit der Soliparty Reise- und Gerichtskosten.
        Lasst uns gemeinsam laut werden und tanzen für <b>GERECHTIGKEIT</b>, gegen Repressionen und für eine <b>OFFENE WELT</b>! Kommt zahlreich und bringt Freund*innen, Familie und/oder wen ihr sonst so mögt mit.
      </p>
      <p style="margin-top:1em;">
        Einen Überblick über den Mapuche Konflikt findet ihr <a @click="openWebsiteNewTab('https://berkleycenter.georgetown.edu/posts/the-mapuche-conflict')">HIER</a>
      </p>

      <p style="margin-top:2em;"><b>
        Partyfacts: 2 Floors // Cocktail Bar // Empanadas
      </b></p>

      <img src="~/assets/soli-djanes.png" class="footerPic">


      <section class="info">
        <div class="infoBox">

        </div>
        <div class="infoBox">

        </div>
        <div class="infoBox">

        </div>
      </section>
    </section>

  </section>
</template>

<script>
export default {
  methods: {
    openWebsiteNewTab(link) {
      window.open(link, "_blank");
    }
  }
}


</script>

<style>
p {
  white-space: pre-line;
}
.galleryContainer {
  display: flex;
  justify-content: space-between;
  width: 100%;
  flex-wrap: wrap;
}

.galleryImage {
  display: flex;
  height: 25em;
}
.video-container {
  position: relative;
  padding-bottom: 54%;
  padding-top: 30px;
  height: 0;
  overflow: hidden;
}

.video-container iframe,
.video-container object,
.video-container embed {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.headerPic {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 3em;
  width: 40em;
}

.footerPic {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
}

.profile {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 3em;
  margin-bottom: 1em;
  width: 30em;
  border-radius: 50%;
}

.pageWrapper {
  padding: 3em;
  min-height: 100vh;
}

.info {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  background-color: white;
}

.infoBox {
  width: 35em;
}
.headingInfobox {
  margin-bottom: 1em;
}
.subHeadingInfobox {
  margin-bottom: 0.5em;
}

#containerProfile {
  overflow: hidden;         /*  clip the excess when child gets bigger than parent  */
}
#containerProfileOld img {
  display: block;
}
#containerProfileOld:hover img {
  transform: scale(1.7);
  transform-origin: 50% 50%;
}
@media screen and (min-width: 1600px) {

}
@media screen and (max-width: 880px) {
  .headerPic {
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 3em;
    width: 20em;
  }
  .galleryContainer {
    display: flex;
    justify-content: space-around;
    width: 100%;
    flex-wrap: wrap;
  }
  .galleryImage {
    display: flex;
    padding-top: 1em;
    width: 100%;
    height: 100%;
  }
  .profile {
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-top: 3em;
    margin-bottom: 1em;
    width: 25em;
    border-radius: 50%;
  }
  .footerPic {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
  }
  .pageWrapper {
    padding: 2em;
    min-height: 100vh;
    width: 100vw;
    max-width: 100%;
    margin: 0;
  }
}

</style>
