<template >
  <section class="products">
    <titles subTitle="Our Products" title="Baked Fresh Every Morning" />
    <article class="products__content">
      <product-card :products="products" >
    </article>
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
          img: "/src/assets/images/products/item1.png",
          category: "Bakery",
          name: "Homemade Bread",
          desc: "Flows by their place and supplies it with the necessary regelialia.",
          price: "$9",
        },
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