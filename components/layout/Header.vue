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
            <nuxt-link to="/about" :class="isAboutPage">About</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/works" :class="isWorksPage">Works</nuxt-link>
          </li>
          <li class="l-header__listItem">
            <nuxt-link to="/blog" :class="isBlogPage">Blog</nuxt-link>
          </li>
        </ul>
      </nav>
      <div class="l-header__sns">
        <ul class="l-header__icons">
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
export default {
  computed: {
    isAboutPage() {
      return {
        'l-header__active': this.$route.path.includes('about'),
        'l-header__link': true
      }
    },
    isWorksPage() {
      return {
        'l-header__active': this.$route.path.includes('work'),
        'l-header__link': true
      }
    },
    isBlogPage() {
      return {
        'l-header__active': this.$route.path.includes('blog'),
        'l-header__link': true
      }
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/mixin.scss';

.l-header {
  &__container {
    width: 240px;
    height: 100%;
    padding: 0 20px;
    text-align: center;

    @include mobile {
      width: 100%;
    }
  }

  &__img {
    width: 120px;
    border-radius: 50%;
  }

  &__title {
    @include text-primary;

    margin-top: 8px;
    font-size: 18px;
  }

  &__nav {
    margin-top: 12px;
  }

  &__link {
    @include text-accent;

    display: inline-block;
    width: 120px;
    padding: 12px 0;
    font-weight: bold;
    text-align: center;
  }

  &__active {
    &::before {
      content: '🐧 ';
      transform: scale(-1, 1);
    }

    &::after {
      content: ' 🐧';
    }
  }

  &__icons {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 12px;
  }

  &__icon {
    width: 24px;
    margin: 12px;
  }
}
</style>
