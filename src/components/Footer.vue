<template>
  <footer>
    <div class="container-link clearfix">
      <div class="sx">
        <div class="space"></div>
        <div class="link-footer">
          <h1>titolo</h1>
          <h4><a href="#">cose</a></h4>

          <h1>titolo</h1>
          <h4><a href="#">cose</a></h4>
        </div>

        <div class="link-footer">
          <h1>titolo</h1>
          <h4><a href="#">cose</a></h4>
        </div>

        <div class="link-footer">
          <h1>titolo</h1>
          <h4><a href="#">cose</a></h4>
        </div>
      </div>
      <div class="dx">
          <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
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
a {
  text-decoration: none;
  color: grey;
}
li {
  list-style-type: none;
  margin-left: 0;
}
.clearfix {
  content: "";
  display: table;
  clear: both;
}
.container-link {
  height: 300px;
  width: 100%;
  background-image: url("../assets/img/footer-bg.jpg");
}
.end {
  background-color: rgba(48, 48, 48, 255);
  height: 80px;
  width: 100%;
}
.sx {
  display: flex;
  float: left;
  height: 100%;
  width: 50%;
}
.dx {
  float: left;
  height: 100%;
  width: 50%;
}
.space {
  width: 50%;
}
.link-footer {
  text-align: left;
  margin: 0 10px;

  h1 {
    color: white;
    font-size: 20px;
  }
  h4 {
    color: white;
    margin: 2px 0;
  }
}

.dx,img{
        height: 50%;
        width: 50%;
}
</style>
