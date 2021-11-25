<template>
  <main>
    <div class="series">
        <img :src="details.thumb" alt="">
        <div class="nomeserie">
        <h4>{{details.series}}</h4>
        </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "Newseries",
  props: {
      details: Object
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.series{    
    height: 100px;
    width: calc(100% / 6);
    img{
        object-fit: contain;
        max-width: 100%;

    }
    h4{
        color: white;
    }
}
</style>
