<template>
  <footer class="footer">
    <div class="container footer__container">
      <div class="footer__wrapper">
        <div class="footer__main">
          <div class="footer__left">
            <h3 class="footer__title">&lt;/ NNGROUP.studio /></h3>
          </div>

          <div class="footer__right">
            <h3 class="footer__subtitle">SOCIAL</h3>
            <form class="footer__form">
              <img src="/sms-tracking.svg" alt="" class="footer__form-icon">
              <input placeholder="Enter Your Email" type="email" class="footer__form-input">
              <button class="footer__form-submit" type="submit">
                <img src="/arrow-right.svg" alt="" class="footer__form-submit-icon">
              </button>
            </form>
            <ul class="footer__socials">
              <li class="footer__socials-item">
                <a href="#" class="footer__socials-link">
                  <img src="/telegram.svg" alt="" class="footer__socials-icon">
                </a>
              </li>
              <li class="footer__socials-item">
                <a href="#" class="footer__socials-link">
                  <img src="/discord.svg" alt="" class="footer__socials-icon">
                </a>
              </li>
              <li class="footer__socials-item">
                <a href="#" class="footer__socials-link">
                  <img src="/whatsapp.svg" alt="" class="footer__socials-icon">
                </a>
              </li>
              <li class="footer__socials-item">
                <a href="#" class="footer__socials-link">
                  <img src="/github.svg" alt="" class="footer__socials-icon">
                </a>
              </li>
              <li class="footer__socials-item">
                <a href="#" class="footer__socials-link">
                  <img src="/instagram.svg" alt="" class="footer__socials-icon">
                </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="footer__decor"></div>
        <p class="footer__copy">nngroup.studio@2024 <span>- All Rights Reserved</span></p>
      </div>
    </div>
  </footer>
</template>

<script setup>

</script>

<style scoped>
.footer__wrapper {
  border-radius: 30px;
  background: var(--color-tertiary);
  padding: 40px;
  padding-bottom: 12px;
  padding-top: 30px;
}

.footer__main {
  display: flex;
  justify-content: space-between;
}


.footer__title {
  color: var(--color-btns);
  font-family: 'Aldrich', sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: 2.16px;
}

.footer__text {
  max-width: 400px;
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
}

.footer__text-span {
  color: var(--color-primary);
}

.footer__decor {
  background: url('/footer-decor.svg');
  background-repeat: no-repeat;
  background-size: contain;
  width: 100%;
  height: 7px;
  padding-left: 10px;
  margin-top: 20px;
  margin-bottom: 12px;
}

.footer__subtitle {
  color: var(--color-btns);
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: 13px;
}

.footer__copy {
  color: var(--color-btns);
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: 1.26px;
  text-align: center;
}

.footer__form {
  position: relative;
  padding-bottom: 3px;
  display: flex;
  align-items: end;
  gap: 9px;
  max-width: fit-content;
}

.footer__form::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 1px;
  left: 0;
  bottom: 0;
  border-radius: 30px;
  background: rgba(25, 25, 25, 0.50);
}

.footer__form-icon {
  width: 18px;
  height: 18px;
}

.footer__form-submit-icon {
  width: 17px;
  height: 17px;
}

.footer__form-input {
  max-width: 113px;
  height: 17px;
  background: none;
  border: none;
  outline: none;
  padding: 2px 0;
  display: block;
  color: rgba(25, 25, 25, 0.50);
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  font-style: normal;
  font-weight: 400;
  line-height: 13px;
}

.footer__form-input::placeholder {
  color: rgba(25, 25, 25, 0.50);
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  font-style: normal;
  font-weight: 400;
  line-height: 13px;
}

.footer__form-submit {
  border: none;
  background: none;
  outline: none;
  cursor: pointer;
  width: 17px;
  height: 17px;
}

.footer__socials {
  display: flex;
  align-items: center;
  gap: 10px;
}

.footer__socials-item {
  border-radius: 100px;
  border: 1px solid rgba(25, 25, 25, 0.50);
  width: 30px;
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer__right {
  padding-right: 35px;
  display: flex;
  align-items: center;
  gap: 20px;
}

@media(max-width: 1100px) {
  .footer__right {
    padding-right: 0;
  }

  .footer__main {
    gap: 40px;
  }
}

@media(max-width: 1000px) {
  .footer__decor {
    display: none;
  }

  .footer__copy {
    margin-top: 60px;
  }

  .footer__main {
    flex-direction: column;
  }

  .footer__wrapper {
    padding: 30px;
    padding-top: 40px;
  }
}

@media(max-width: 768px) {
  .footer__logo {
    font-size: 20px;
  }

  .footer__right {
    flex-direction: column;
  }

  .footer__title {
    text-align: center;
  }

  .footer__container {
    padding-right: 0;
    padding-left: 0;
  }

  .footer__wrapper {
    border-radius: 0px;
  }
}

@media(max-width: 540px) {
  .footer__title {
    font-size: 20px;
  }

  .footer__copy span {
    display: none;
  }
}
</style>