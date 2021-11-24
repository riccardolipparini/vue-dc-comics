<template>
    <main>
        <div class="container"></div>
        <div class="utilities">
            <a href="#">
            <div class="object">
            <img src="" alt="">
            <h1></h1>
            </div>
            </a>
        </div>
    </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
    height: 100px;
    width: 100%;
    background-color: black;
}
.utilities{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 200px;
    background-color: rgba(2,130,249,255);
    h1{
        color: white;
    }
}
.object{
    display: flex;
    justify-content: center;
    align-items: center;
    h1{
        margin: 0 10px;
    }
}

</style>
