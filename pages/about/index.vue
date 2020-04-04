<template>
  <main class="p-about">
    <div class="p-about__container">
      <div class="p-about__head">
        <h2 class="p-about__title">Manaki Ikeda</h2>
        <p class="p-about__work">front-end engineer</p>
        <p class="p-about__location">
          <font-awesome-icon icon="map-marker-alt" /> Osaka,Japan
        </p>
      </div>
      <div class="p-about__hero">
        <img
          class="p-about__img"
          src="@/assets/image/about/about__hero.png"
          alt="著者の画像"
        />
      </div>
      <div class="p-about__infos">
        <div class="p-about__info">
          <h3 class="p-about__subTitle">Work</h3>
          <p>
            現在大学を休学中の休学インターンニートです。フロントエンジニアを目指して大阪のweb制作会社でアルバイトをさせていただいています。
            特にウェブサービス開発に興味があり。自分でも製作中です。
          </p>
        </div>

        <div class="p-about__info">
          <h3 class="p-about__subTitle">経歴</h3>
          <div class="p-about__history">
            <time>1998年</time>
            <p>兵庫県に爆誕！</p>
          </div>
          <div class="p-about__history">
            <time>2016年</time>
            <p>
              University of Nothern Iowaに入学
            </p>
          </div>
          <div class="p-about__history">
            <time>2019年</time>
            <p>休学インターンニートになる</p>
          </div>
        </div>

        <div class="p-about__info">
          <h3 class="p-about__subTitle">好きなこと</h3>
          <p>焼肉、ゲーム、web制作、</p>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
@import '@/assets/scss/mixin.scss';

.p-about {
  @include mobile {
    text-align: center;
  }

  &__container {
    padding: 0 20px;

    @include mobile {
      text-align: center;
      widows: 100%;
    }
  }

  &__head {
    @include mobile {
      text-align: center;
    }
  }

  &__work {
    margin-top: 2px;
  }

  &__location {
    margin-top: 8px;
  }

  &__hero {
    margin-top: 12px;
  }

  &__img {
    width: 100%;
    max-width: 640px;
  }

  &__subTitle {
    margin-top: 24px;
    margin-bottom: 8px;
  }

  &__history {
    margin-top: 12px;
  }
}
</style>
