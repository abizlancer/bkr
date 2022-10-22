<template >
  <section class="products container">
    <titles subTitle="Our Products" title="Baked Fresh Every Morning" />
    <div class="products__content">
      <product-card class="products__card--big" :key="0">
        <div class="products__card--img">
          <img src="/src/assets/images/products/item1.png" alt="products img">
        </div>
       <div class="products__card--big--info">
          <small>Bakery</small>
          <h3>Homemade Bread</h3>
          <div class="price">
            <p>Flows by their place and supplies it with the necessary regelialia.</p>
            <h3>$9</h3>
          </div>
       </div>
      </product-card>
      <product-card v-for="(product, key) in products" :key="key + 1" >
        <div class="products__card--img">
          <img :src="product.img" alt="products img">
        </div>
        <div class="products__card--info">
          <small>{{ product.category }}</small>
          <h3>{{ product.name }}</h3>
          <h4>{{ product.price }}</h4>
        </div>
      </product-card>
    </div>
  </section>
</template>

<script>
import Titles from "../Titles.vue"
import ProductCard from './ProductsCard.vue'

export default {
  name: 'Products',
  components: {
    Titles,
    ProductCard,
  },
  data() {
    return {
      products: [
        {
          img: "/src/assets/images/products/item2.png",
          category: "Bakery",
          name: "Bread",
          price: "$5",
        },
        {
          img: "/src/assets/images/products/item3.png",
          category: "Pastry",
          name: "Cupcake",
          price: "$3",
        },
        {
          img: "/src/assets/images/products/item4.png",
          category: "Sweet",
          name: "Biscuits",
          price: "$2",
        },
        {
          img: "/src/assets/images/products/item5.png",
          category: "Pastry",
          name: "Brioche",
          price: "$5",
        },
      ]
    }
  },
}
</script>