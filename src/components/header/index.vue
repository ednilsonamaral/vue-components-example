<template>
  <nav class="navbar navbar-default navbar-fixed-top">
    <div class="container-fluid">
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed" @toggle="onToggleMenu" @click="toggle">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>

        <a class="navbar-brand link-img-header" href="/">
          <img src="../../assets/img/vue-logo.png" class="img-header">
          <p>Componentes</p>
        </a>
      </div>


      <div class="collapse navbar-collapse" :class="{ in: isOpen }">
        <ul class="nav navbar-nav">
          <router-link to="/sobre" tag="li">
            <a>Sobre</a>
          </router-link>


          <router-link to="/contato" tag="li">
            <a>Contato</a>
          </router-link>
        </ul>
      </div><!-- /.navbar-collapse -->
    </div><!-- /.container-fluid -->
  </nav>
</template>

<script>
export default {
  data () {
    return {
      isOpen: false
    }
  },

  methods: {
    toggle () {
      this.$emit('toggle')
    },

    onToggleMenu () {
      this.isOpen = !this.isOpen
    }
  }
}
</script>

<style scoped>
.link-img-header{
  display: flex;
  align-items: center;
  /*padding: 0;*/
  margin: 0;
}

.link-img-header p{
  margin: 0;
  color: #2c3e50;
}

.link-img-header p:hover{
  color: #41b883;
}

.img-header{
  width: 40px;
  height: 40px;
}
</style>
