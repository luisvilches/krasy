<template>
  <div class="banner">
    <div class="overlay"></div>
    <br>
    <br>
    <br>
    <br>
    <div class="container text-left">
      <div class="row">
        <div class="col-md-6">
          <h1>Recibe los mejores servicios de belleza</h1>
          <h2>en tu casa, oficina, hotel o donde sea.</h2>
          <br>
          <button class="btn btn-danger">¡Agenda tu servicio {{name}}!</button>
        </div>
        <div class="col-md-6"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'banner',
  data () {
    return {
      name: 'Krasy'
    }
  }
}
</script>


<style scoped>
  .banner{
    background-image: url('.././assets/banner.png');
    background-attachment: fixed;
    width: 100%;
    min-height: 600px;
    background-repeat: no-repeat;
    margin-top:-20px; 
    padding: 60px;
    background-size: cover;
  }
  h1{
    margin-top: 50px;
  }

  @media(max-width:991px){
    h1{
      margin-top: -25px;
    }
  }
  h1,h2{
    text-align: left;
    color: #fff;
  }

  button{
    padding: 10px 40px;
  }

  .overlay{
    background-color: #222534;
    position: absolute;
    top: 0;
    left: 0;
    display: block;
    width: 100%;
    height: 580px;
    opacity: 0.6;
    filter: alpha(opacity=40);
    z-index: 0;
  }
</style>
