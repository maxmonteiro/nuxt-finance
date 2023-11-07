<template>
  <div>
    <div class="container mx-auto">
      <h1 class="text-lg font-bold">Serviços</h1>

      <nuxt-link to="/servicos/desenvolvimento-de-sites">
        Desenvolvimento de Sites
      </nuxt-link>

      <nuxt-link to="/servicos/marketing-digital">
        Marketing Digital
      </nuxt-link>

      <br>

      <nuxt-child />
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

  methods: {

  }
}
</script>
