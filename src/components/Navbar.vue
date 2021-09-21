<template>
  <header class="d-flex justify-content-between py-3 px-5 align-items-center">
    <div class="d-flex align-items-center">
      <g-image
        alt="Example image"
        src="~/assets/images/logo.svg"
        class="me-5"
        width="50"
      />
      <div class="d-none d-md-flex align-items-center">
        <g-link to="/" class="text-dark me-4 text-decoration-none">Home</g-link>
        <g-link to="/blog" class="text-dark me-4 text-decoration-none"
          >Blog</g-link
        >
        <g-link to="/recipes" class="text-dark text-decoration-none"
          >Recipes</g-link
        >
      </div>
    </div>
    <div class="d-none d-md-flex aling-items-center">
      <div class="d-flex flex-row aling-items-center">
        <p class="d-flex align-items-center pe-3">Follow us</p>
        <span class="d-flex align-items-center">|</span>
        <a href="" class="d-flex align-items-center text-dark ms-3"
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-youtube"
          >
            <path
              d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.25 29 29 0 0 0-.46-5.33z"
            ></path>
            <polygon
              points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02"
            ></polygon></svg
        ></a>
      </div>
      <button class="btn btn-dark ms-4">Contact us</button>
    </div>
    <svg @click="toggleNav(true)" class="pointer d-block d-md-none feather feather-menu" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="3" y1="12" x2="21" y2="12"></line><line x1="3" y1="6" x2="21" y2="6"></line><line x1="3" y1="18" x2="21" y2="18"></line></svg>
    <div v-if="mobileNavVisible" class="mobile-nav d-block d-md-none position-absolute h-100 bg-dark">
        <svg @click="toggleNav(false)" class="pointer text-white position-absolute feather feather-x" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>
        <div class="d-flex flex-column align-items-end mt-5 pt-5 pe-5">
            <g-link to="/" class="text-white mb-4 text-decoration-none">Home</g-link>
            <g-link to="/blog" class="text-white mb-4 text-decoration-none"
            >Blog</g-link
            >
            <g-link to="/recipes" class="text-white mb-4 text-decoration-none"
            >Recipes</g-link
            >
        </div>
    </div>
  </header>
</template>

<script>
export default {
    data() {
        return {
            mobileNavVisible: false,
        }
    },
    methods: {
        toggleNav(param) {
            this.mobileNavVisible = param;
        }
    },
}
</script>

<style scoped lang="scss">
.mobile-nav {
    width: 380px;
    max-width: 100%;
    right: 0;
    top: 0;

    .feather-x {
        z-index: 1;
        right: 45px;
        top: 30px;
    }
}
</style>