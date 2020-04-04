<template>
  <header class="l-header">
    <div class="l-header__container">
      <div class="l-header__head">
        <img
          src="@/assets/image/header/header__logo.png"
          alt="ウェブサイトロゴ"
          class="l-header__img"
        />
        <h1 class="l-header__title">MANAKI IKEDA</h1>
      </div>
      <nav class="l-header__nav">
        <ul class="l-header__list">
          <li class="l-header__listItem">
            <nuxt-link to="/" class="l-header__link">About</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/" class="l-header__link">Works</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/" class="l-header__link">Blog</nuxt-link>
          </li>
        </ul>
      </nav>
      <div class="l-header__sns">
        <ul class="l-header__icons">
          <li>
            <a href=""><font-awesome-icon icon="fab fa-github"/></a>
          </li>
          <li>
            <a href="">
              <img
                class="l-header__icon"
                src="@/assets/image/header/header__instagram.svg"
                alt="インスタロゴ"
              />
            </a>
          </li>
          <li>
            <a href="">
              <img
                class="l-header__icon"
                src="@/assets/image/header/header__twitter.svg"
                alt="Twitterロゴ"
              />
            </a>
          </li>
          <li>
            <a href="">
              <img
                class="l-header__icon"
                src="@/assets/image/header/header__github.svg"
                alt="githubロゴ"
              />
            </a>
          </li>
          <li>
            <a href="">
              <img
                class="l-header__icon"
                src="@/assets/image/header/header__youtube.svg"
                alt="youtubeロゴ"
              />
            </a>
          </li>
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
    width: 400px;
    height: 100%;
    padding: 0 40px;
    text-align: center;
  }

  &__img {
    width: 200px;
    border-radius: 50%;
  }

  &__title {
    @include text-primary;

    margin-top: 24px;
    font-size: 24px;
  }

  &__nav {
    margin-top: 24px;
  }

  &__link {
    @include text-accent;

    display: inline-block;
    width: 120px;
    padding: 12px 0;
    font-weight: bold;
    text-align: center;
  }

  &__icons {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 24px;
  }

  &__icon {
    width: 24px;
    margin: 12px;
  }
}
</style>
