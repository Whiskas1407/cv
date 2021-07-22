<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__contacts">
        <a href="https://telegram.me/bogdansinitsya" target="_blank" class="footer__contacts-link">Telegram</a>
        <a href="https://github.com/Whiskas1407" target="_blank" class="footer__contacts-link">GitHub</a>
        <h2 class="footer__logo">BOGDAN SINITSYA</h2>
        <a href="https://www.instagram.com/bn.evrey.sinitsya/" target="_blank" class="footer__contacts-link">Instagram</a>
        <a href="https://www.linkedin.com/in/bogdan-sinitsya-3708531b4/" target="_blank" class="footer__contacts-link">LinkedIn</a>
      </div>
    </div>
  </footer>
</template>
<style lang="scss">
.footer {
  width: 100%;
  border-top: .2rem solid $brown;
  padding: 2rem 0;
  &__contacts {
    display: flex;
    align-items: center;
    justify-content: space-between;
    transition: .3s;
    &-link {
      text-transform: uppercase;
      font-family: Raleway-Medium;
      &:hover {
        color: $brown;
      }
    }
  }
  &__logo {
    font-family: ZenTokyo;
    font-size: 3.6rem;
    cursor: pointer;
  }
}
</style>
