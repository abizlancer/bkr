<template>
  <nav class="nav">
    <nav class="nav--content container">
      <article class="nav-links">
        <a href="#!" class="logo">bkr</a>
        <ul class="nav-list">
          <li v-for="(link, key) in list" :key="key">
            <a href={{link.link}}>{{link.text}}</a>
          </li>
        </ul>
      </article>
      <a href="#!" class="nav-btn">contacts</a>
      <div class="burger">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </nav>
  </nav>
</template>
<script>
export default {
  name: 'Navbar',
  data() {
    return {
      list: [
        {
          link: '#!',
          text: 'About',
        },
        {
          link: '#!',
          text: 'Products',
        },
        {
          link: '#!',
          text: 'Recipes',
        },
      ]
    }
  },
}
</script>