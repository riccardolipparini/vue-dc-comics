<template>
  <footer>
    <div class="container-link clearfix">
      <div class="sx">
        <div class="space"></div>
        <div class="link-footer">
          <h1>DC COMICS</h1>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>

          <h1>SHOP</h1>
          <h4><a href="#">cose</a></h4>
          <h4><a href="#">ciao</a></h4>
        </div>

        <div class="link-footer">
          <h1>DC</h1>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
        </div>

        <div class="link-footer">
          <h1>SITES</h1>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
          <h4><a href="#">ciao</a></h4>
        </div>
      </div>
      <div class="dx">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="end"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data(){
      return {
          info: [
              {
                  url: "#",
                  text: "ciaoooo"
              },
              {
                  url: "#",
                  text: "hola"
              },
              {
                  url: "#",
                  text: "como estas"
              },
              {
                  url: "#",
                  text: "sas"
              },
              {
                  url: "#",
                  text: "sahas"
              },
              
          ]
      }
  }
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
  width: 20%;
}
.link-footer {
  text-align: left;
  margin: 30px 10px;

  h1 {
    color: white;
    font-size: 15px;
  }
  h4 {
    color: white;
    margin: 2px 0;
  }
}

.dx,
img {
  height: 50%;
  width: 50%;
}
</style>
