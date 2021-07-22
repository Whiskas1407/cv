<template>
  <section class="home container" id="home">
    <div class="home__info">
      <h1 class="home__info-title">Front-End Developer</h1>
      <ul class="home__info-ul">
        <li class="home__info-list">
          <p class="home__info-subtitle">Опыт разработки <span>2г 3м 1д 10ч 52м 11с</span></p>
        </li>
      </ul>
      <button class="home__info-button button__light">Связатся</button>
    </div>
    <img src="/home-page.png" class="home__image">
  </section>
</template>
<style lang="scss">
.home {
  display: grid;
  grid-template-columns: 91rem 59rem;
  align-items: center;
  padding-top: 5rem;
  &__info {
    &-title {
      font-size: 5rem;
    }
    &-ul {
      margin-top: 2rem;
    }
    &-subtitle {
      font-size: 2.2rem;
      width: 75rem;
      margin: 1.5rem 0;
      font-family: Arial;
    }
    &-button {
      margin-top: 2rem;
      font-size: 1.8rem;
    }
  }
  &__image {
    width: 60rem;
  }
}
@media screen and (max-width: 460px) {
  .home {
    grid-template-columns: 36rem;
    &__info {
      text-align: center;
      margin-top: 5rem;
      &-subtitle {
        text-align: left;
      }
    }
    &__image {
      display: none;
    }
  }
}
</style>
