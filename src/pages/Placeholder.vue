<template>
  <Layout>
    <div class="container">
      <g-image alt="Example image" src="~/assets/images/logo.svg" width="135" />
      <h1>We are coming soon</h1>
      <p>We are preparing something amazing and exciting for you.</p>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Countedmacros.com'
  }
}
</script>

<style lang="scss">
* {
  font-family: 'DM Sans', sans-serif;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

h1 {
  font-size: 60px;
  margin-bottom: 0;
  text-align: center;
}

p {
  margin-top: 0;
  text-align: center;
  margin-bottom: 0;
}
</style>
