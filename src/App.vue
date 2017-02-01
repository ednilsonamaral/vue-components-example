<template>
  <div class="container-fluid">
    <div class="row">
      <!-- <img src="./assets/img/vue-logo.png"> -->

      <RootHeader></RootHeader>
    </div>

    <div class="container" style="margin-top: 100px;">
        <router-view></router-view>
    </div>

    <div class="row">
      <div class="col-lg-12">
        <RootFooter></RootFooter>
      </div>
    </div>
  </div><!-- fim do /.container-fluid da página toda -->
</template>

<script>
import RootHeader from './components/header'
import RootFooter from './components/footer'

export default {
  name: 'app',
  components: { RootHeader, RootFooter }
}
</script>

<style lang="sass" src="assets/css/scss/app.scss"></style>
