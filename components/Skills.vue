<template>
  <section class="skills" id="skills">
    <div class="container">
      <div class="skills__content">
        <h2 class="skills__title">Мои навыки</h2>
        <div class="skills__items">
          <div class="skills__item">
            <img src="/html-5.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">HTML <br>( PUG )</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/css-3.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">CSS <br>( Perfect Pixel )</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/sass.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">SASS</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/js.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">JavaScript <br>( TypeScript )</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/vue.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">VueJs <br> ( VueX )</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star.svg" alt="star">
              <img src="/star.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/nuxt-js.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">NuxtJs</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star.svg" alt="star">
            </div>
          </div>
          <div class="skills__item">
            <img src="/github.svg" alt="skill" class="skills__item-image">
            <p class="skills__item-title">GIT</p>
            <div class="skills__item-stars">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star-active.svg" alt="star">
              <img src="/star.svg" alt="star">
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss">
.skills {
  padding: 5rem 0;
  &__title {
    text-align: center;
    font-size: 3.6rem;
    padding-bottom: 1rem;
    border-bottom: .2rem solid $brown;
  }
  &__items {
    display: grid;
    grid-template-columns: 25rem 25em 25rem 25rem;
    grid-column-gap: 16.6rem;
    grid-row-gap: 5rem;
    padding-top: 5rem;
  }
  &__item {
    padding: 2rem;
    width: 20rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    &-image {
      width: 12rem;
    }
    &-title {
      text-align: center;
      font-size: 2.6rem;
      padding-top: 1rem;
    }
    &-stars {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 100%;
      padding-top: 2rem;
      img {
        width: 3rem;
      }
    }
  }
}
@media screen and (max-width: 460px) {
  .skills {
    &__items {
      display: grid;
      grid-template-columns: 36rem;
      grid-column-gap: 0;
      grid-row-gap: 5rem;
      padding-top: 5rem;
      justify-items: center;
    }
  }
}
</style>
