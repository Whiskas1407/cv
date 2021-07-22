<template>
  <section class="portfolio container">
    <h2 class="portfolio__title">Успешные проекты</h2>
    <div class="portfolio__projects">
      <a href="https://csgo.expert" class="portfolio__project" target="_blank">
        <div class="portfolio__project-content">
        </div>
        <h3 class="portfolio__project-title">CSGO.EXPERT</h3>
        <p class="portfolio__project-subtitle">Торговая площадка с возможностю обмена скинов CS:GO за реальные деньги</p>
      </a>
      <a href="https://cybertime.finance" class="portfolio__project" target="_blank">
        <div class="portfolio__project-content">
        </div>
        <h3 class="portfolio__project-title">CYBERTIME.FINANCE</h3>
        <p class="portfolio__project-subtitle">Личная монета! Возможность купить на аукционне и не только.</p>
      </a>
      <a href="https://mojam.co/home" class="portfolio__project" target="_blank">
        <div class="portfolio__project-content">
        </div>
        <h3 class="portfolio__project-title">MOJAM</h3>
        <p class="portfolio__project-subtitle">Информационный сайт компании с актуальными вакансиями и блоге коллектива</p>
      </a>
    </div>
  </section>
</template>
<style lang="scss">
.portfolio {
  padding: 5rem 0;
  &__title {
    text-align: center;
    font-size: 3.6rem;
    padding-bottom: 1rem;
    border-bottom: .2rem solid $brown;
  }
  &__projects {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding-top: 5rem;
  }
  &__project {
    width: 100rem;
    min-height: 55rem;
    height: auto;
    background-repeat: no-repeat;
    background-size: 100%;
    position: relative;
    align-items: center;
    margin-bottom: 5rem;
    cursor: pointer;
    transition: .3s;
    &:hover .portfolio__project-content {
      opacity: 0;
    }
    &:hover > .portfolio__project-title {
      display: none;
    }
    &:hover > .portfolio__project-subtitle {
      display: none;
    }
    &:nth-child(1) {
      background-image: url("/csgo.png");
    }
    &:nth-child(2) {
      background-image: url("/cybertime.png");
    }
    &:nth-child(3) {
      background-image: url("/mojam.png");
    }
    &-content {
      position: absolute;
      width: 100%;
      height: 100%;
      background: #000;
      opacity: .5;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
    }
    &-title {
      font-size: 3.2rem;
      text-align: center;
      position: absolute;
      top: 3rem;
      left: 3rem;
    }
    &-subtitle {
      font-size: 2.2rem;
      text-align: center;
      position: absolute;
      right: 3rem;
      bottom: 3rem;
    }
  }
}
@media screen and (max-width: 460px) {
  .portfolio {
    &__project {
      width: 36rem;
      background-size: cover;
      background-position: left;
    }
  }
}
</style>
