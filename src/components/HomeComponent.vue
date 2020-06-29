<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand to="/">Home</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item to="/blog">Blog</b-nav-item>
          <b-nav-item to="/services">Services</b-nav-item>
          <b-nav-item to="/contact">Contact</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <div class="row">
      <div class="col-md-4 col-lg4" 
      v-for="(data,index) in products" :key="index">
        <img :src="data.image" class="img-fluid" />
        <h3>{{data.productTitle}}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home Component",

  data: () => ({
    products: [
      {
        productTitle: "ABCN",
        image: require("../assets/images/product1.jpg"),
        productId: 1
      },
      {
        productTitle: "KARMA",
        image: require("../assets/images/product2.jpg"),
        productId: 2
      },
      {
        productTitle: "Tino",
        image: require("../assets/images/product3.jpg"),
        productId: 3
      },
      {
        productTitle: "EFG",
        image: require("../assets/images/product4.jpg"),
        productId: 4
      },
      {
        productTitle: "MLI",
        image: require("../assets/images/product5.jpg"),
        productId: 5
      },
      {
        productTitle: "Banans",
        image: require("../assets/images/product6.jpg"),
        productId: 6
      }
    ]
  })
};
</script>

<style scoped>
 .row {
   margin: 8px 15px;
 }

</style>