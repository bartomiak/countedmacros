<template>
  <div class="layout">
    <Navbar />
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import Navbar from '~/components/Navbar.vue'

export default {
  components: {
    Navbar,
  }

}
</script>

<style lang="scss">
.layout {
  height: 90vh;
}
</style>