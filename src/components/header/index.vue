<template>
  <nav class="navbar navbar-default navbar-fixed-top">
    <div class="container-fluid">
      <a class="navbar-brand link-img-header" href="/">
        <img src="../../assets/img/vue-logo.png" class="img-header">
        <p>Componentes</p>
      </a>

      <div class="collapse navbar-collapse" id="barraFixaTop">
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
