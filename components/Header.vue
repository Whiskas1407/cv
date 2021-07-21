<template>
  <header class="header container">
    <div class="header__navigation">
      <div class="header__navigation-link">
        <ul class="header__navigation-link-ul">
          <li class="header__navigation-link-list">
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li class="header__navigation-link-list">
            <nuxt-link to="/">Skills</nuxt-link>
          </li>
        </ul>
      </div>
      <h2 class="header__navigation-logo">BOGDAN SINITSYA</h2>
      <div class="header__navigation-link">
        <ul class="header__navigation-link-ul">
          <li class="header__navigation-link-list">
            <nuxt-link to="/">Portfolio</nuxt-link>
          </li>
          <li class="header__navigation-link-list">
            <nuxt-link to="/">Contacts</nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>
<style lang="scss">
.header {
  padding-top: 2rem;
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
        width: 30rem;
      }
      &-list {
        a {
          transition: .3s;
          &:hover {
            color: $gray;
          }
        }
      }
    }
  }
}
</style>
