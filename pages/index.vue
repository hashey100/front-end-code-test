<template>
  <section class="container">
    <div>
      <app-logo class="logo" />
      <h1 class="title">
        Wi5 Front-end Code Test
      </h1>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-size: 40px;
  color: #0b2c48;
  letter-spacing: 0.02em;
}

.logo {
  width: 150px;
  margin-bottom: 5px;
}

</style>

