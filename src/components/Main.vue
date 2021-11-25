<template>
  <main>
    <div class="container0"></div>

    <div class="container">
        <Newseries v-for="serie, i in series" :key="i" :details="serie"/>
    </div>

    <div class="utilities">
      <div class="object" v-for="(buy, i) in things" :key="i">
        <img :src="require(`../assets/img/${buy.img}`)" />
        <h4>{{ buy.text }}</h4>
      </div>
    </div>
  </main>
</template>
import Newseries from './components/Newseries.vue';

<script>
import Newseries from './Newseries.vue';
export default {
  components: { Newseries },
  name: "Main",
  data() {
    return {
      things: [
        {
          url: "#",
          img: "buy-comics-digital-comics.png",
          text: "ciaoooo",
        },
        {
          url: "#",
          img: "buy-comics-merchandise.png",
          text: "hola",
        },
        {
          url: "#",
          img: "buy-comics-shop-locator.png",
          text: "como estas",
        },
        {
          url: "#",
          img: "buy-comics-subscriptions.png",
          text: "sas",
        },
        {
          url: "#",
          img: "buy-dc-power-visa.svg",
          text: "sahas",
        },
      ],
      series: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container0 {
  height: 200px;
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: 100%;
  background-repeat: no-repeat;
  position: relative;
  width: 100%;
}
.container {
    display: flex;
    flex-wrap: wrap;
  background-color: black;
}
.utilities {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 200px;
  background-color: rgba(2, 130, 249, 255);
  h4 {
    color: rgb(255, 255, 255);
    margin: 0 20px;
  }
}
.object {
  width: calc(100% / 4);
  display: flex;
  justify-content: center;
  align-items: center;
  h1 {
    margin: 0 10px;
  }
  img {
    max-width: 20%;
  }
}
</style>
