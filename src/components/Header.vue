<template>
  <header>
    <div id="navbar">
      <img src="../assets/img/dc-logo.png" alt="logo DC" />
      <ul>
        <li v-for="links, i in navs" :key="i">
          <a :href="links.url" :class="links.active ? `active` : ``">{{links.text}}</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data(){
    return {
      navs: [
        {
          text: "Characters",
          url: "#",
          active: false,
        },
        {
          text: "Comics",
          url: "#",
          active: true,
        },
        {
          text: "Movies",
          url: "#",
          active: false,
        },
        {
          text: "Tv",
          url: "#",
          active: false,
        },
        {
          text: "Games",
          url: "#",
          active: false,
        },
        {
          text: "News",
          url: "#",
          active: false,
        },
        {
          text: "Collectons",
          url: "#",
          active: false,
        },
        {
          text: "Movies",
          url: "#",
          active: false,
        },
        {
          text: "Fan",
          url: "#",
          active: false,
        },
        {
          text: "Info",
          url: "#",
          active: false,
        }
      ]
    }
  }
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
a:hover{
  background-color: lightblue;
  padding: 10px;
}
.active{
  background-color: lightblue;
  padding: 10px;
}

</style>
