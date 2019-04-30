<template>
  <section class="container">
    <section class="container-wrapper">
      <Cover/>
      <Info/>
      <Footer/>
    </section>
  </section>
</template>

<script>
import Cover from '../components/Cover'
import Info from '../components/Info'
import Footer from '../components/Footer'

export default {
  components: {
    Cover,
    Info,
    Footer
  }
}
</script>

<style>

/*  Color Palette Notes
#677517
#528BCC
#ADC23A
#8F261D
#75251D

#347529
#183613
#50B63F
#57C244
#469C36

#84CC3D

#8D6FC9
*/

.container {
  width: 100vw;
  max-width: 100%;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  overflow-x: hidden;
}

.container .container-wrapper {
 /* TODO container wrapper */
}

.links {
  padding-top: 15px;
}
</style>
