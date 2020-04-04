<template>
  <header class="l-header">
    <div class="l-header__container">
      <div class="l-header__head">
        <img src="@/assets/image/header__logo.png" alt="ウェブサイトロゴ" />
        <h1 class="l-header__title">MANAKI IKEDA</h1>
      </div>
      <nav class="l-header__nav">
        <ul class="l-header__list">
          <li class="l-header__listItem">
            <nuxt-link to="/">About</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/">Works</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/">Blog</nuxt-link>
          </li>
        </ul>
      </nav>
      <div class="l-header__sns">
        <ul class="l-header__lists">
          <li>
            <a href=""><font-awesome-icon icon/></a>
          </li>
          <li><a href=""></a></li>
          <li><a href=""></a></li>
          <li><a href=""></a></li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';

.l-header {
  &__container {
    @extend .c-container;
  }
}
</style>
