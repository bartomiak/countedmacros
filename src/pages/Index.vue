<template>
  <Layout>
    <section class="hero">
      <div class="container">
        <div class="row pb-5">
          <div class="col-lg-10">
            <h1 class="mt-5 pt-5 text-start mb-3">
              If you’re ready to change your relationship with food for the better, follow us @healthfirst for daily meal plans and updates.
            </h1>
            <p class="text-start mb-5 pb-5">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor adhuc invidunt.</p>
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <div class="row py-5 my-5">
          <div class="col-lg-5 d-flex flex-column align-items-start justify-content-center pe-5">
            <h2 class="text-start mb-3">It's time to kick start a new lifestyle. Start eating, feeling & living better today. Build good habits with us in no time.</h2>
            <p class="text-start">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna velum aliquyam erat, sed diam voluptua. At vero eos et mea accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est lorem ipsum.</p>
            <button class="btn btn-dark mt-4">Read more about us</button>
            
          </div>
          <div class="col-lg-7">
            <g-image
                alt="Example image"
                src="~/assets/images/pasta.jpg"
                class="me-5 img-fluid"
              />
          </div>
        </div>
      </div>
    </section>
    <section>
      <div class="container">
        <h2 class="text-center mb-0">Latest on blog</h2>
        <p class="mb-5">Lorem ipsum dolor sit amet</p>
        <div class="row mb-5 pb-5">
          <div v-for="post in 4" :key="post" class="col-sm-6 col-lg-3 d-flex flex-column align-itesm-start px-3">
            <g-image
                alt="Example image"
                src="~/assets/images/pasta.jpg"
                class="me-5 img-fluid"
              />
              <small class="category-badge align-self-start mt-3 px-1">DIET</small>
              <h4 class="text-start mt-3">Fitness Recipes: Healthy Food for Any Workout</h4>
              <p class="text-start text-small">Aenean sollicitudin, lorem quis bibendum auctor, nisi elit consequat ipsum, nec sagittis sem nibh.</p>
              <p class="text-start mt-3 border-bottom pb-2 align-self-start">Read more</p>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-dark">
      <div class="container">
        <div class="row py-5">
          <div class="col-lg-7 py-5">
            <g-image
                alt="Example image"
                src="~/assets/images/pasta.jpg"
                class="me-5 img-fluid"
              />
          </div>
          <div class="col-lg-5 ps-5 d-flex flex-column align-items-start justify-content-center">
            <h2 class="mb-5 text-white text-start">Check out latest YouTube video:</h2>
            <h3 class="text-start text-white">Zucchini pasta bolognese</h3>
            <p class="text-start text-white">Lorem ipsum dolor sit amet ipsum dolor sit amet </p>
            <button class="btn btn-success mt-5 py-2">Subscribe</button>
          </div>
        </div>
      </div>
    </section>
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
