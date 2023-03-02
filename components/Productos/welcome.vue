<template>
     <div fluid class="banner">
        <img src="../../static/img/banner/productos.png" alt="Banner imagen">
        <div class="overlay"></div>
        <h1>{{ texto }}</h1>
  </div>
</template>

<script>

export default {
props: {
  texto:{
    type: String,
    require: true
  }
}

}

</script>