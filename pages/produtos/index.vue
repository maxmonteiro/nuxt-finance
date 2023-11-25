<template>
  <div>
    <div class="container mx-auto">
      <h1 class="text-lg font-bold">Produtos</h1>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eligendi optio recusandae officia, possimus corrupti velit aperiam consequuntur nesciunt quibusdam eaque quidem labore unde fugiat magni aliquid, numquam magnam? Assumenda, voluptatum.</p>

    <br>
    <br>

    <div v-for="product in products" :key="product.id"
      class="border-b border-gray-400 py-3"
    >
      {{  product.title }}
    </div>

    </div>
  </div>
</template>

<script>
export default {
  name: '',

  data() {
    return {

    }
  },

  async asyncData({ $axios }) {
    const products = await $axios.$get('https://jsonplaceholder.typicode.com/posts?_limit=3')

    return {
      products
    }
  },

  methods: {

  }
}
</script>
