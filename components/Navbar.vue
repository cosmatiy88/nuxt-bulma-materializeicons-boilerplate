<template>
  <nav class="navbar is-link" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <img src="https://cdn.bitrix24.ru/b10161553/landing/cad/cadb752d64005db0cc861f3bf1212585/1.png" width="112" height="28">
      </a>

      <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>


      <div class="navbar-end">
          <nuxt-link class="navbar-item" to="/">
            Главная
          </nuxt-link>
        <nuxt-link class="navbar-item" to="/photo">
          Фотографии
        </nuxt-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
name: "Navbar"
}
</script>

<style scoped>

</style>
