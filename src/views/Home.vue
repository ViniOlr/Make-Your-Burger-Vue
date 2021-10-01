<template>
  <Banner />
  <h1 class="title">Monte o seu hambúrguer</h1>
  <BurgerForm />
</template>

<script>
import Banner from '../components/Banner.vue'
import BurgerForm from '../components/BurgerForm.vue'

export default {
  name: "Home",
  components: {
    Banner,
    BurgerForm
  }
}
</script>

<style scoped>

</style>
