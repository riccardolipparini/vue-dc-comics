<template>
    <footer>
        <div class="container-link clearfix">
            <div class="sx"></div>
            <div class="dx"></div>
        </div>
        <div class="end"></div>
    </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.clearfix{
    content: "";
    display: table;
    clear: both;
}
.container-link{
    height: 300px;
    width: 100%;
    background-image:url("../assets/img/footer-bg.jpg");
}
.end{
    background-color: rgba(48,48,48,255);
    height: 80px;
    width: 100%;
}
.sx{
    float: left;
    background-color: yellow;
    height: 100%;
    width: 50%;
}
.dx{
    float: left;
    background-color:cadetblue;
    height: 100%;
    width: 50%;
}


</style>
