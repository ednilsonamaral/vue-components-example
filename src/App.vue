<template>
  <div class="container-fluid">
    <div class="row">
      <!-- <img src="./assets/img/vue-logo.png"> -->

      <RootHeader></RootHeader>
    </div>

    <div class="container" style="margin-top: 50px;">
        <router-view></router-view>
    </div>
  </div><!-- fim do /.container-fluid da página toda -->
</template>

<script>
import RootHeader from './components/header'

export default {
  name: 'app',
  components: { RootHeader }
}
</script>

<style lang="sass" src="assets/css/scss/app.scss"></style>
