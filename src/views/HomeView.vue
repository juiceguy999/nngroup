<script setup>
import TheTabs from '@/components/TheTabs.vue';

</script>

<template>
  <main>
    <section class="hero">
      <div class="container hero__container">
        <div class="hero__left">
          <p class="hero__logo">&lt;/ NNGROUP /></p>
          <p class="hero__text">
            СТУДИЯ <span class="hero__text-decor">***</span> <br> <span class="hero__text-span">СОЗДАНИЯ</span> <br>
            ПРОЕКТОВ <span class="hero__text-mobile"><br/> NNGROUP</span>
          </p>
          <div class="hero__mobile">
            <img src="/hero-mobile.webp" alt="" class="hero__mobile-img">
            <a href="#" class="hero__link">
              <img src="/yt-preview.jpg" alt="" class="hero__link-img">
              <span class="hero__link-info">
                <span class="hero__link-text">/YouTube</span>
                <img src="/yt-icon.svg" alt="" class="hero__link-icon">
              </span>
            </a>
          </div>
          <div class="hero__descr">
            <p class="hero__descr-brand">NNGROUP</p>
            <p class="hero__descr-text">
              Воплощаем в жизнь самые <span class="hero__descr-span">разнообразные</span> идеи и концепции, <span
                class="hero__descr-span">независимо</span> от их <span class="hero__descr-span">характера</span> и
              сложности.
            </p>
          </div>
          <div class="hero__info">
            <div class="hero__info-team">
              <div class="hero__info-img-group">
                <img src="/expert-1.jpg" alt="" class="hero__info-img">
                <img src="/expert-2.jpg" alt="" class="hero__info-img">
                <img src="/expert-3.jpg" alt="" class="hero__info-img">
              </div>
              <p class="hero__info-number">38+</p>
            </div>
            <p class="hero__info-text">
              Талантливых и опытных специалистов, которые превратят вашу идею в успешный проект
            </p>
          </div>
        </div>
        <div class="hero__right">
          <img src="/hero.webp" alt="">
          <div class="hero__decor">
            <img src="/eye.svg" alt="" class="hero__decor-img">
            <div class="hero__decor-svg">
            <svg
              width="281"
              height="281"
              viewBox="0 0 100 100"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                id="circlePath"
                class="circle-path"
                d="
                  M 50, 50
                  m -40, 0
                  a 40,40 0 1,0 80,0
                  a 40,40 0 1,0 -80,0
                "
              />
              <text class="circular-text">
                <textPath href="#circlePath">
                  • NNGROUP COMMUNITY • NNGROUP COMMUNITY • NNGROUP COMMUNITY
                </textPath>
              </text>
            </svg>
            </div>
          </div>
          <button class="hero__btn">
            <img src="/chevrons.svg" alt="" class="hero__btn-icon">
          </button>
          <a href="#" class="hero__link">
            <img src="/yt-preview.jpg" alt="" class="hero__link-img">
            <span class="hero__link-info">
              <span class="hero__link-text">/YouTube</span>
              <img src="/yt-icon.svg" alt="" class="hero__link-icon">
            </span>
          </a>
        </div>
      </div>
    </section>

    <section class="tabs">
      <div class="container tabs__container">
        <TheTabs></TheTabs>
      </div>
    </section>

    <section class="roadmap">
      <div class="roadmap__container container">
        <div class="roadmap-up">
          <div class="roadmap-item">
            <img src="/teacher.svg" alt="" class="roadmap-icon">
            <p class="roadmap-text">Обучение программированию</p>
          </div>
          <div class="roadmap-item">
            <img src="/shopping-cart.svg" alt="" class="roadmap-icon">
            <p class="roadmap-text">Маркет разработок</p>
          </div>
          <div class="roadmap-item">
            <img src="/favorite-chart.svg" alt="" class="roadmap-icon">
            <p class="roadmap-text">Продвижение и реклама</p>
          </div>
        </div>
        <div class="roadmap-down">
          <div class="roadmap-item">
            <img src="/coin.svg" alt="" class="roadmap-icon">
            <p class="roadmap-text">Финансирование стартапов</p>
          </div>
          <div class="roadmap-item">
            <img src="/code.svg" alt="" class="roadmap-icon">
            <p class="roadmap-text">Разработка цифровых продуктов</p>
          </div>
        </div>
      </div>
    </section>

    <section class="info">
      <div class="container info__container">
        <div class="info__links">
          <div class="info__links-top">
            <a href="#" class="info__links-item">Карьера <div class="info__links-icon"><img src="/arrow-small.svg" alt="" class="info__links-icon-img"></div></a>
            <a href="#" class="info__links-item">Инвестиции <div class="info__links-icon"><img src="/arrow-small.svg" alt="" class="info__links-icon-img"></div></a>
          </div>
          <div class="info__links-down">
            <a href="#" class="info__links-item">Стартапы <div class="info__links-icon"><img src="/arrow-small.svg" alt="" class="info__links-icon-img"></div></a>
            <a href="#" class="info__links-item">О нас  <div class="info__links-icon"><img src="/arrow-small.svg" alt="" class="info__links-icon-img"></div></a>
          </div>
        </div>
        <div class="info__items">
          <div class="info__item">
            <p class="info__item-text">Инвестиций <br> в стартапы</p>
            <p class="info__item-subtext">$300к+</p>
            <a href="#" class="info__item-link"><img src="/dark-arrow.svg" alt="" class="info__item-icon"></a>
            <div class="info__item-decor info__item-decor--right"><div class="info__item-decor-circle"></div></div>
          </div>
          <div class="info__item info__item--mid">
            <p class="info__item-text">Наши заслуги <br> и достижения</p>
            <a href="#" class="info__item-link"><img src="/dark-chevron.svg" alt="" class="info__item-icon"></a>
            <div class="info__item-decor info__item-decor--up"><div class="info__item-decor-circle"></div></div>
          </div>
          <div class="info__item">
            <p class="info__item-text">Реализовано проектов </p>
            <p class="info__item-subtext">68+</p>
            <a href="#" class="info__item-link"><img src="/dark-arrow.svg" alt="" class="info__item-icon"></a>
            <div class="info__item-decor info__item-decor--left"><div class="info__item-decor-circle"></div></div>
          </div>
          <div class="info__decor">
            <img src="/eye.svg" alt="" class="info__decor-img">
            <svg
              width="160"
              height="160"
              viewBox="0 0 100 100"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                id="circlePath"
                class="circle-path"
                d="
                  M 50, 50
                  m -40, 0
                  a 40,40 0 1,0 80,0
                  a 40,40 0 1,0 -80,0
                "
              />
              <text class="circular-text">
                <textPath href="#circlePath">
                  • NNGROUP • NNGROUP • NNGROUP
                </textPath>
              </text>
            </svg>
          </div>
        </div>
      </div>
    </section>

    <section class="portfolio">
      <div class="container portfolio__container">
        <h2 class="portfolio__title">Портфолио</h2>
        <div class="portfolio__grid">
          <div class="portfolio__card portfolio__card--one">
            <div class="portfolio__card-header">
              <div class="portfolio__card-space"></div>
              <div class="portfolio__card-action">
                <div class="portfolio__card-link--test">
                  <img src="/card-icon.svg" alt="" class="portfolio__card-link-icon">
                </div>
              </div>
            </div>
            <div class="portfolio__card-img-box">
              <img src="/card-img-1.png" alt="" class="portfolio__card-img">
            </div>
            <div class="portfolio__card-body">
              <div class="portfolio__card-info">
                <h3 class="portfolio__card-title portfolio__card-title--light">METASPINS</h3>
                <div class="portfolio__card-tags">
                  <div class="portfolio__card-tag portfolio__card-tag--light">Backend / Frontend</div>
                  <div class="portfolio__card-tag portfolio__card-tag--light">UX / UI Design</div>
                  <div class="portfolio__card-tag portfolio__card-tag--light">Promotion</div>
                </div>
              </div>
            </div>
            <div class="portfolio__card-bg"></div>
          </div>
          <div class="portfolio__card portfolio__card--two">
            <div class="portfolio__card-header">
              <div class="portfolio__card-space"></div>
              <div class="portfolio__card-action">
                <div class="portfolio__card-link--test">
                  <img src="/card-icon.svg" alt="" class="portfolio__card-link-icon">
                </div>
              </div>
            </div>
            <div class="portfolio__card-img-box">
              <img src="/card-img-2.png" alt="" class="portfolio__card-img">
            </div>
            <div class="portfolio__card-body">
              <div class="portfolio__card-info">
                <h3 class="portfolio__card-title portfolio__card-title--light">GARANTEX</h3>
                <div class="portfolio__card-tags">
                  <div class="portfolio__card-tag portfolio__card-tag--light">Backend / Frontend</div>
                  <div class="portfolio__card-tag portfolio__card-tag--light">UX / UI Design</div>
                </div>
              </div>
            </div>
            <div class="portfolio__card-bg"></div>
          </div>
          <div class="portfolio__card portfolio__card--three">
            <div class="portfolio__card-header">
              <div class="portfolio__card-space"></div>
              <div class="portfolio__card-action">
                <div class="portfolio__card-link--test">
                  <img src="/card-icon.svg" alt="" class="portfolio__card-link-icon">
                </div>
              </div>
            </div>
            <div class="portfolio__card-img-box">
              <img src="/card-img-3.png" alt="" class="portfolio__card-img">
            </div>
            <div class="portfolio__card-body">
              <div class="portfolio__card-info">
                <h3 class="portfolio__card-title">To the sun</h3>
                <div class="portfolio__card-tags">
                  <div class="portfolio__card-tag">Backend / Frontend</div>
                  <div class="portfolio__card-tag">UX / UI Design</div>
                  <div class="portfolio__card-tag">Promotion</div>
                </div>
              </div>
            </div>
            <div class="portfolio__card-bg"></div>
          </div>
          <div class="portfolio__card portfolio__card--four">
            <div class="portfolio__card-header">
              <div class="portfolio__card-space"></div>
              <div class="portfolio__card-action">
                <div class="portfolio__card-link--test">
                  <img src="/card-icon.svg" alt="" class="portfolio__card-link-icon">
                </div>
              </div>
            </div>
            <div class="portfolio__card-img-box">
              <img src="/card-img-4.png" alt="" class="portfolio__card-img">
            </div>
            <div class="portfolio__card-body">
              <div class="portfolio__card-info">
                <h3 class="portfolio__card-title">uran.music</h3>
                <div class="portfolio__card-tags">
                  <div class="portfolio__card-tag">Backend / Frontend</div>
                  <div class="portfolio__card-tag">UX / UI Design</div>
                </div>
              </div>
            </div>
            <div class="portfolio__card-bg"></div>
          </div>
        </div>
        <a href="#" class="portfolio__link">
          Ознакомиться с полным портфолио
          <div class="portfolio__link-icon">
            <img src="/arrow.svg" alt="" class="portfolio__link-icon-img">
          </div>
        </a>
      </div>
    </section>



  </main>
</template>

<style>


.hero {
  padding-bottom: 80px;
  padding-top: 17px;
}

.hero::before {
  content: '';
  position: absolute;
  z-index: -1;
  top: 0;
  left: 0;
  background: url('/sphere-hero.svg');
  background-size: cover;
  background-repeat: no-repeat;
  width: 500px;
  height: 500px;
}

.hero::after {
  content: '';
  position: absolute;
  z-index: -1;
  top: 242px;
  right: 0;
  background: url('/sphere-hero-second.svg');
  background-size: cover;
  background-repeat: no-repeat;
  width: 577px;
  height: 832px;
}

.hero__container {
  display: flex;
  justify-content: space-between;
  align-items: end;
}

.hero__logo {
  color: var(--color-btns);
  margin-bottom: 100px;
  font-family: 'Aldrich', sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: 2.16px;
}

.hero__text {
  font-family: 'Days One', sans-serif;
  color: var(--color-btns);
  font-size: 64px;
  font-style: normal;
  font-weight: 400;
  line-height: 104px;
  text-transform: uppercase;
}

.hero__text-span {
  color: var(--color-secondary);
}

.hero__text-decor {
  margin-left: 27px;
  color: var(--color-secondary);
  padding: 12px 44px;
  border-radius: 100px;
  border: 1px solid var(--color-secondary);
  height: 50px;
  display: inline-block;
  line-height: 43px;
  transform: translateY(20%);
}

.hero__descr {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-bottom: 60px;
}

.hero__descr-text {
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  max-width: 275px;
}

.hero__descr-span {
  color: var(--color-primary);
}

.hero__descr-brand {
  font-family: 'Days One', sans-serif;
  color: var(--color-tertiary);
  font-size: 50px;
  font-style: normal;
  font-weight: 400;
  line-height: 104px;
  text-transform: uppercase;
}

.hero__text-mobile {
  color: var(--color-tertiary);
  font-family: 'Days One', sans-serif;
  font-size: 25px;
  font-style: normal;
  font-weight: 400;
  line-height: 60px;
  text-transform: uppercase;
  display: none;
}

.hero__info {
  max-width: fit-content;
  position: relative;
  padding: 20px 0;
  display: flex;
  align-items: center;
  gap: 23px;
}

.hero__info::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 7px;
  background-image: url('/hero-decor.svg');
  background-size: cover;
}

.hero__info::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 7px;
  background-image: url('/hero-decor.svg');
  background-size: cover;
}

.hero__info-team {
  display: flex;
  align-items: center;
  gap: 25px;
}

.hero__info-img-group {
  display: flex;
  align-items: center;
  gap: 5px;
}

.hero__info-img {
  width: 70px;
  height: 70px;
  border-radius: 20px;
}

.hero__info-img:not(:first-child) {
  margin-left: -10px;
}

.hero__info-number {
  color: var(--color-btns);
  font-family: 'Days One';
  font-size: 30px;
  font-style: normal;
  font-weight: 400;
  line-height: 43px;
  letter-spacing: 3px;
  text-transform: uppercase;
}

.hero__info-text {
  max-width: 230px;
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
}

.hero__right {
  position: relative;
}

.hero__right img {
  display: block;
}

.hero__decor {
  position: absolute;
  top: 50%;
  left: -150px;
  transform: translateY(-50%);

  width: 271px;
  height: 271px;
  border-radius: 50%;
  border: 1px solid var(--color-btns);
  background: rgba(255, 255, 255, 0.60);
  backdrop-filter: blur(5px);

  display: flex;
  justify-content: center;
  align-items: center;
}

.hero__decor-img {
  width: 180px;
}

.hero__decor-svg {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}

.circle-path {
  fill: transparent;
}

.circular-text {
  fill: #000;
  font-family: 'Inter', sans-serif;
  font-size: 5px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 1px;
  text-transform: uppercase;
}

@-webkit-keyframes rotating {
  from {
    -webkit-transform: translate(-50%,-50%) rotate(0deg);
    -o-transform: translate(-50%,-50%) rotate(0deg);
    transform: translate(-50%,-50%) rotate(0deg);
  }
  to {
    -webkit-transform: translate(-50%,-50%) rotate(360deg);
    -o-transform: translate(-50%,-50%) rotate(360deg);
    transform: translate(-50%,-50%) rotate(360deg);
  }
}
@keyframes rotating {
  from {
    -ms-transform: translate(-50%,-50%) rotate(0deg);
    -moz-transform: translate(-50%,-50%) rotate(0deg);
    -webkit-transform: translate(-50%,-50%) rotate(0deg);
    -o-transform: translate(-50%,-50%) rotate(0deg);
    transform: translate(-50%,-50%) rotate(0deg);
  }
  to {
    -ms-transform: translate(-50%,-50%) rotate(360deg);
    -moz-transform: translate(-50%,-50%) rotate(360deg);
    -webkit-transform: translate(-50%,-50%) rotate(360deg);
    -o-transform: translate(-50%,-50%) rotate(360deg);
    transform: translate(-50%,-50%) rotate(360deg);
  }
}

.hero__decor-svg {
  -webkit-animation: rotating 180s linear infinite;
  -moz-animation: rotating 180s linear infinite;
  -ms-animation: rotating 180s linear infinite;
  -o-animation: rotating 180s linear infinite;
  animation: rotating 180s linear infinite;
}

.hero__btn {
  position: absolute;
  left: 74px;
  bottom: 0;

  width: 32px;
  height: 70px;
  border-radius: 100px;
  background: var(--color-tertiary);
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  border: none;
}

.hero__btn-icon {
  width: 11px;
}

.hero__link {
  position: absolute;
  bottom: 2px;
  right: 0;

  display: flex;
  align-items: center;
  gap: 9px;
  width: 136px;
  height: 70px;
  padding-left: 1px;
  padding-right: 10px;
  border-radius: 15px;
  background: var(--color-tertiary);
}

.hero__link-img {
  width: 68px;
  height: 68px;
  border-radius: 14px;
}

.hero__link-info {
  display: flex;
  flex-direction: column;
  gap: 10px;
  align-items: center;
}

.hero__link-text {
  color: var(--color-btns);
  text-align: center;
  font-family: 'Ubuntu Mono', sans-serif;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.hero__link-icon {
  width: 24px;
  height: 24px;
}

.hero__mobile {
  display: none;
  position: relative;
  margin-bottom: 30px;
  max-width: fit-content;
}

@media(max-width: 1100px) {
  .hero {
    padding-bottom: 130px;
  }

  .hero__info-team {
    flex-direction: column-reverse;
    gap: 8px;
    align-items: start;
  }

  .hero__text-decor {
    display: none;
  }

  .hero__decor {
    left: -30px;
  }
}

@media(max-width: 1003px) {
  .hero__mobile {
    display: block;
  }

  .hero__right {
    display: none;
  }

  .hero__container {
    justify-content: center;
  }

  .hero__logo {
    display: none;
  }

  .hero {
    padding-top: 88px;
  }

  .hero__text {
    font-size: 40px;
    line-height: 60px;
    margin-bottom: -55px;
  }

  .hero__descr-decor {
    display: none;
  }

  .hero__info-text {
    max-width: 175px;
  }

  .hero__info-text > br {
    display: none;
  }

  .hero__info-img-group {
    gap: 0;
  }

  .hero__info-img {
    border: none;
    width: 60px;
    height: 60px;
    border-radius: 20px;
  }

  .hero__info-img:not(:first-child) {
    margin-left: -10px;
  }

  .hero__descr-text {
    max-width: 360px;
  }

  .hero__descr {
    margin-bottom: 30px;
  }

  .hero__link {
    width: 130px;
    height: 60px;
    gap: 12px;
  }

  .hero__link-img {
    width: 58px;
    height: 58px;
  }

  .hero__link-info {
    gap: 8px;
  }

  .hero__descr-brand {
    display: none;
  }

  .hero__text-mobile {
    display: inline;
  }
}

@media(max-width: 768px) {
  .hero::before {
    width: 262px;
    height: 563px;
    background: url('/sphere-hero-mobile.svg');
  }

  .hero::after {
    background: url('/sphere-hero-second-mobile.svg');
    width: 133px;
    height: 640px;
    top: 817px;
  }
}

.roadmap {
  padding-top: 27px;
  padding-bottom: 127px;
  min-height: 245px;
  background-image: url('/roadmap-bg.svg');
  background-repeat: no-repeat;
  background-position-x: 13vw;
  max-width: 100%;
}

.roadmap-up {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: -8px;
}

.roadmap-item {
  position: relative;
  z-index: -1;
  border-radius: 20px;
  border: 1px solid var(--color-primary);
  box-shadow: 0px 0px 4px 1px rgba(136, 146, 238, 0.50) inset;
  background: rgba(255, 255, 255, 0.01);
  backdrop-filter: blur(10px);
  display: flex;
  align-items: center;
  gap: 30px;
  padding: 16px 28px;
}

.roadmap-icon {
  width: 22px;
  height: 22px;
}

.roadmap-text {
  color: #3C3D3D;
  text-align: center;
  font-size: 12px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  text-transform: uppercase;
}

.roadmap-down {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 810px;
  margin: 0 auto;
  margin-top: 95px;
}

@media(max-width: 1700px) {
  .roadmap {
    background-position-x: 7vw;
  }
}

@media(max-width: 1500px) {
  .roadmap {
    background-position-x: 0vw;
  }
}

@media(max-width: 1300px) {
  .roadmap {
    background-position-x: -7vw;
  }
}

@media(max-width: 1100px) {
  .roadmap {
    display: none;
  }
}

.portfolio {
  padding-top: 200px;
  padding-bottom: 100px;
}

.portfolio__title {
  color: var(--color-btns);
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 60px; 
  text-transform: uppercase;
  margin-bottom: 40px;
}

.portfolio__grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
}

.portfolio__card {
  position: relative;
  min-height: 400px;
}

.portfolio__card-bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  background: url('/portfolio-card-bg-1.svg');
  background-repeat: no-repeat;
  background-position: center;
}

.portfolio__card--one .portfolio__card-bg {
  background: url('/portfolio-card-bg-1.svg');
  background-repeat: no-repeat;
  background-position: center;
}

.portfolio__card--two .portfolio__card-bg {
  background: url('/portfolio-card-bg-2.svg');
  background-repeat: no-repeat;
  background-position: center;
}

.portfolio__card--three .portfolio__card-bg {
  background: url('/portfolio-card-bg-3.svg');
  background-repeat: no-repeat;
  background-position: center;
}

.portfolio__card--four .portfolio__card-bg {
  background: url('/portfolio-card-bg-4.svg');
  background-repeat: no-repeat;
  background-position: center;
}

.portfolio__card-link {
  position: absolute;
  top: 0;
  right: 0;
  width: 120px;
  height: 60px;
  border-radius: 16px;
  background: var(--color-btns);
  display: flex;
  justify-content: center;
  align-items: center;
}

.portfolio__card-link-icon {
  width: 30px;
  height: 30px;
}

.portfolio__card-title {
  font-family: 'Days One';
  color: var(--color-btns);
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px;
  text-transform: uppercase;
  margin-bottom: 20px;
}

.portfolio__card-title--light {
  color: #fff;
}

.portfolio__card-tags {
  display: flex;
  align-items: center;
  gap: 20px;
}

.portfolio__card-tag {
  border-radius: 100px;
  border: 1px solid var(--color-btns);
  padding: 10px 20px;
  color: var(--color-btns);
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px;
  background: rgba(255, 255, 255, 0.01);
  backdrop-filter: blur(4px);
}

.portfolio__card-tag--light {
  color: #fff;
  border-color: #fff;
}

.portfolio__card-img-box {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1;
  transform: scale(0.9);
}


.portfolio__card-info {
  position: relative;
  z-index: 1;
}

.portfolio__link {
  position: relative;
  border-radius: 20px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);

  color: #FFF;
  text-align: center;
  font-size: 15px;
  font-style: normal;
  font-weight: 500;
  line-height: 13px;
  padding: 22px 68px;
  display: block;
  max-width: 580px;
  margin-top: 30px;
  margin-left: auto;
}

.portfolio__link-icon {
  width: 46px;
  height: 46px;
  position: absolute;
  right: 5px;
  top: 50%;
  transform: translateY(-50%);
  border-radius: 16px;
  background: var(--color-tertiary);

  display: flex;
  justify-content: center;
  align-items: center;
}

.portfolio__card-header {
  display: flex;
  justify-content: space-between;
  height: 70px;
  gap: 10px;
}

.portfolio__card-space {
  position: relative;
  width: 100%;
  background: #97C3E9;
  border-radius: 10px 10px 0px 0px;
}

.portfolio__card-space::after {
  content: '';
  position: absolute;
  right: -20px;
  bottom: 0;
  width: 20px;
  height: 20px;
  background: transparent;
  border-radius: 0px 0px 0px 20px;
  box-shadow: -5px 5px 0 5px #97C3E9;
}

.portfolio__card-action {
  width: 155px;
  padding-bottom: 10px;
}

.portfolio__card-link--test {
  /* width: 120px; */
  /* height: 60px; */
  width: 100%;
  height: 100%;
  border-radius: 16px;
  background: var(--color-btns);
  display: flex;
  justify-content: center;
  align-items: center;
}

.portfolio__card-body {
  background: #97C3E9;
  border-radius: 0px 10px 10px 10px;
  height: calc(100% - 70px);
  display: flex;
  align-items: end;
  padding-left: 30px;
  padding-bottom: 20px;
  padding-right: 30px;
}

.portfolio__card--two .portfolio__card-body, .portfolio__card--two .portfolio__card-space {
  background: var(--color-primary);
}

.portfolio__card--two .portfolio__card-space::after {
  box-shadow: -5px 5px 0 5px var(--color-primary);
}

.portfolio__card--three .portfolio__card-body, .portfolio__card--three .portfolio__card-space {
  background: var(--color-tertiary);
}

.portfolio__card--three .portfolio__card-space::after {
  box-shadow: -5px 5px 0 5px var(--color-tertiary);
}

.portfolio__card--four .portfolio__card-body, .portfolio__card--four .portfolio__card-space {
  background: var(--color-quaternary);
}

.portfolio__card--four .portfolio__card-space::after {
  box-shadow: -5px 5px 0 5px var(--color-quaternary);
}

.portfolio__card-img {
  max-width: 100%;
}

@media(max-width: 1200px) {
  .portfolio__grid {
    grid-template-columns: 1fr;
  }

  .portfolio__card .portfolio__card-bg {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
    height: 100%;
    background: url('/portfolio-card-mobile.svg');
    background-repeat: no-repeat;
    background-position: left;
  }
}

@media(max-width: 768px) {
  .portfolio__card-action {
    width: 82px;
  }

  .portfolio__card-header {
    height: 63px;
  }

  .portfolio__card-tags {
    gap: 10px;
    flex-wrap: wrap;
  }

  .portfolio__link {
    padding-left: 48px;
    padding-right: 68px;
  }

  .portfolio {
    padding-top: 70px;
    padding-bottom: 70px;
  }

  .portfolio__title {
    font-size: 30px;
    font-style: normal;
    font-weight: 700;
    line-height: 60px;
    text-transform: uppercase;
    margin-bottom: 20px;
  }
}

/* Courses  */

.courses {
  padding-top: 100px;
}

.courses__title {
  color: var(--color-btns);
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 60px;
  text-transform: uppercase;
  margin-bottom: 40px;
}

.courses__card {
  position: relative;
  width: 320px;
  height: 240px;
  background: url('/card-body.svg');
  background-position: center;
  background-repeat: no-repeat;
  padding-left: 16px;
  padding-right: 20px;
  padding-top: 87px;
  padding-bottom: 20px;

  display: flex;
  align-items: center;
  justify-content: space-between;
}

.courses__card-icon {
  position: absolute;
  top: 19px;
  left: 21px;
  width: 30px;
  border-radius: 5px;
}

.courses__card-price {
  position: absolute;
  top: 0;
  left: 82px;
  border-radius: 10px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);
  width: 130px;
  height: 56px;
  padding: 18px 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;

  color: #FFF;
  text-align: center;
  font-family: 'Ubuntu', sans-serif;
  font-size: 14px;
  font-style: normal;
  font-weight: 700;
  line-height: 9px;
}

.courses__card-price-icon {
  width: 20px;
  height: 20px;
}

.courses__card-info {
  position: absolute;
  top: 0;
  right: 0;
  border-radius: 10px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);
  width: 98px;
  height: 56px;
  padding: 18px 14px;
  display: flex;
  align-items: center;
  justify-content: space-between;

  color: #FFF;
  text-align: center;
  font-family: 'Ubuntu', sans-serif;
  font-size: 14px;
  font-style: normal;
  font-weight: 700;
  line-height: 9px;
}

.courses__card-info-icon {
  width: 20px;
  height: 20px;
}

.courses__card-list {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.courses__card-list-item {
  display: flex;
  align-items: center;
  gap: 10px;

  color: var(--color-btns);
  font-family: 'Ubuntu', sans-serif;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 9px;
}

.courses__card-list-icon {
  width: 18px;
  height: 18px;
}

.splide__pagination__page {
  width: 70px;
  height: 6px;
  border-radius: 4px;
  background: #E9E9EA;
  margin: 0;
  margin-left: 10px;
  margin-right: 10px;
  opacity: 1;
}

.splide__pagination__page.is-active {
  transform: none;
  background: #161616;
}

.splide__pagination__page:hover {
  background: #E9E9EA;
}

.splide__pagination__page.is-active:hover {
  background: #161616;
}

.splide__pagination {
  bottom: -36px;
}

@media(max-width: 768px) {
  .courses__title {
    font-size: 30px;
    font-style: normal;
    font-weight: 700;
    line-height: 60px;
    text-transform: uppercase;
    margin-bottom: 20px;
  }

  .splide__pagination__page {
    width: 50px;
  }

  .splide__pagination {
    padding-left: 0;
    padding-right: 0;
  }
}

@media(max-width: 470px) {
  .splide__pagination__page {
    width: 30px;
  }
}

.team {
  padding-top: 110px;
  padding-bottom: 120px;
}

.team__title {
  color: var(--color-btns);
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 60px;
  text-transform: uppercase;
  margin-bottom: 8px;
}

.team__main {
  display: flex;
  justify-content: space-between;
  margin-bottom: 50px;
}

.team__info {
  align-self: end;
  max-width: 439px;
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
}

.team__info-span {
  color: var(--color-primary);
}

.team__items {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.team__items-up {
  display: flex;
  gap: 20px;
}

.team__item {
  padding: 14px 30px;
  border-radius: 40px;
  border: 1px solid var(--color-border);
  background: #FFF;
}

.team__item-text {
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 400;
  line-height: 13px;
}

.team__items-down {
  display: flex;
  gap: 20px;
}

.team__item-span {
  font-weight: 700;
}



.team__card {
  width: 80px;
  height: 80px;
  border-radius: 10px;
}

@media(max-width: 1100px) {
  .team__main {
    flex-direction: column;
    gap: 30px;
  }

  .team__info {
    align-self: start;
  }
}

@media(max-width: 768px) {
  .team {
    padding-bottom: 60px;
  }

  .team__title {
    font-size: 30px;
    font-style: normal;
    font-weight: 700;
    line-height: 60px;
    text-transform: uppercase;
    margin-bottom: 20px;
  }

  .team__items {
    gap: 10px;
  }

  .team__items-up {
    gap: 10px;
    flex-wrap: wrap;
  }

  .team__items-down {
    gap: 10px;
    flex-wrap: wrap;
  }

  .team__item {
    padding: 14px 20px;
  }
}

.info {
  background: url('/decor-bg.svg');
  background-repeat: no-repeat;
  background-position: center;
  min-height: 370px;
}

.info__decor {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  border: 1px solid var(--color-primary);
  background: rgba(255, 255, 255, 0.01);
  box-shadow: 0px 0px 4px 1px rgba(136, 146, 238, 0.50) inset;
  backdrop-filter: blur(10px);
  display: flex;
  justify-content: center;
  align-items: center;
  display: none;
}

.info__decor-img {
  width: 93px;
}

.info__decor > svg {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}

.info__decor .circular-text {
  fill: #000;
  font-family: 'Inter', sans-serif;
  font-size: 6px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 4.6px;
  text-transform: uppercase;
}



.info__items {
  padding: 0 120px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  position: relative;
  bottom: -100px;
}

.info__item {
  position: relative;
  width: 170px;
  height: 170px;
  border-radius: 100px;
  border: 1px solid var(--color-primary);
  background: rgba(255, 255, 255, 0.01);
  box-shadow: 0px 0px 4px 1px rgba(136, 146, 238, 0.50) inset;
  backdrop-filter: blur(5px);
  padding: 20px;
  padding-top: 30px;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  gap: 6px;
}

.info__item-text {
  color: #3C3D3D;
  text-align: center;
  font-size: 12px;
  font-style: normal;
  font-weight: 700;
  line-height: 24px; 
  text-transform: uppercase;
}

.info__item-subtext {
  color: var(--color-primary);
  text-align: center;
  font-size: 22px;
  font-style: normal;
  font-weight: 900;
  line-height: 20px; 
  text-transform: uppercase;
}

.info__item-link {
  display: block;
}

.info__item-icon {
  width: 30px;
  height: 30px;
}

.info__links {
  position: relative;
  top: -30px;
}

.info__links-top {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 240px;

  margin-bottom: 52px;
}

.info__links-item {
  position: relative;
  min-width: 210px;
  border-radius: 48px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);
  padding: 22px;
  padding-right: 50px;

  color: #FFF;
  text-align: center;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 500;
  line-height: 13px; 
}

.info__links-icon {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  right: 5px;

  border-radius: 100px;
  background: var(--color-tertiary);
  width: 46px;
  height: 46px;

  display: flex;
  justify-content: center;
  align-items: center;
}

.info__links-icon-img {
  width: 13px;
  height: 13px;
}

.info__links-down {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.info__item-decor {
  content: '';
  position: absolute;
  width: 27px;
  height: 27px;
  border-radius: 20px;
  background: rgba(136, 146, 238, 0.4);

  display: flex;
  justify-content: center;
  align-items: center;
}

.info__item-decor-circle {
  width: 8px;
  height: 8px;
  border-radius: 20px;
  background: var(--color-primary);
}

.info__item-decor--right {
  right: 23px;
  top: 0px;
}

.info__item-decor--up {
  top: -14px;
  left: 50%;
  transform: translateX(-50%);
}

.info__item-decor--left {
  left: 23px;
  top: 0px;
}

.info__item--mid {
  bottom: -37px;
}

@media(max-width: 1250px) {
  .info__item-decor {
    display: none;
  }
}

@media(max-width: 1003px) {
  .info__links {
    display: none;
  }

  .info__item {
    border-color: var(--color-primary);
    justify-content: center;
    align-items: center;
    gap: 10px;
    width: 160px;
    height: 160px;
    padding: 16px;
  }

  .info__item-link {
    display: none;
  }

  .info__item--mid .info__item-link {
    display: block;
  }

  .info {
    background: url('/decor-bg-mobile.svg');
    background-repeat: no-repeat;
    background-position: center;
    min-height: 630px;
  }

  .info__items {
    padding: 0;
    padding-top: 75px;
    position: static;
    display: grid;
    grid-template-columns: 160px 160px;
    gap: 160px 40px;
    justify-content: center;
  }

  .info__item--mid {
    bottom: 0;
  }

  .hero  {
    padding-bottom: 70px;
  }

  .info__decor {
    display: flex;
  }
}


section.tabs {
  position: relative;
  padding-bottom: 80px;
}

/* section.tabs::before {
  content: '';
  position: absolute;
  z-index: -1;
  top: 150px;
  left: 0;
  background: url('/sphere-tabs.svg');
  background-size: cover;
  background-repeat: no-repeat;
  width: 290px;
  height: 600px;
}

section.tabs::after {
  content: '';
  position: absolute;
  z-index: -1;
  top: 120px;
  right: 0;
  background: url('/sphere-tabs-second.svg');
  background-size: cover;
  background-repeat: no-repeat;
  width: 286px;
  height: 600px;
} */

@media(max-width: 768px) {
  section.tabs::before {
  display: none;
}

section.tabs::after {
  display: none;
}
}
</style>
