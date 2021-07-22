<template>
  <header class="header container">
    <div class="header__navigation">
      <div class="header__navigation-link">
        <ul class="header__navigation-link-ul">
          <li class="header__navigation-link-list">
            <p @click="goto('home')">На вверх</p>
          </li>
          <li class="header__navigation-link-list">
            <p @click="goto('skills')">Мои навыки</p>
          </li>
        </ul>
      </div>
      <h2 class="header__navigation-logo">BOGDAN SINITSYA</h2>
      <div class="header__navigation-link">
        <ul class="header__navigation-link-ul">
          <li class="header__navigation-link-list">
            <p @click="goto('portfolio')">Успешные проекты</p>
          </li>
          <li class="header__navigation-link-list">
            <p @click="goto('footer')">Контакты</p>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  methods: {
    goto(refName) {
      let el = document.getElementsByClassName(refName)[0];
      if (el) {
        el.scrollIntoView({behavior: 'smooth'});
      }
    }
  }
}
</script>
<style lang="scss">
.header {
  position: fixed;
  padding: 2rem 21rem;
  top: 0;
  z-index: 2;

  background: $default;
  &__navigation {
    display: flex;
    align-items: center;
    justify-content: space-between;
    &-logo {
      font-family: ZenTokyo;
      font-size: 3.6rem;
      cursor: pointer;
    }
    &-link {
      &-ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 40rem;
      }
      &-list {
        p {
          transition: .3s;
          cursor: pointer;
          &:hover {
            color: $gray;
          }
        }
      }
    }
  }
}
@media screen and (max-width: 460px) {
  .header {
    &__navigation {
      &-link {
        display: none;
      }
      &-logo {
        font-size: 2.6rem;
        margin: 0 auto;
      }
    }
  }
}
</style>
