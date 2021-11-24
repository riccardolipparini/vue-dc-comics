<template>
  <header>
    <div id="navbar">
      <img src="../assets/img/dc-logo.png" alt="logo DC" />
      <ul>
        <li><a href="#">Ciao</a></li>
        <li><a href="#">Ciao</a></li>
        <li><a href="#">Ciao</a></li>
        <li><a href="#">Ciao</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#navbar {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 100px;
  width: 100%;
  li {
    display: inline-block;
    margin: 0 20px;
    a {
      text-decoration: none;
      color: black;
    }
  }
}
</style>
