<script setup>
import { ref } from 'vue';
import { onClickOutside } from '@vueuse/core';

const props = defineProps(['currentInnerTab', 'currentTab']);
const menuStatus = ref(false);
const menu = ref(null);

onClickOutside(menu, event => {
  if(menuStatus.value) {
    menuStatus.value = false;
  }
});
</script>

<template>
  <div class="subtabs">
    <div class="subtabs__nav">
      <div class="subtabs__menu">
        <button ref="menu" @click="menuStatus = !menuStatus" class="subtabs__menu-btn">{{ props.currentTab.name }} <img :class="{active: menuStatus}" src="/tabs-mobile-chevron.svg" alt="" class="subtabs__menu-icon"></button>
        <div :class="{active: menuStatus}" class="subtabs__list">
          <button v-for="subtab in currentTab.cases" :class="['subtabs__btn', { active: currentInnerTab === subtab }]"
            @click="$emit('changeTab', subtab)">
            {{ subtab.name }}
            <img src="/tabs-arrow.svg" alt="" class="subtabs__btn-icon">
          </button>
        </div>
      </div>
      <a href="#" class="subtabs__link">
        Связаться
        <span class="subtabs__link-icon">
          <img src="/tabs-arrow-dark.svg" alt="" class="subtabs__link-img">
        </span>
      </a>
    </div>
    <div class="subtabs__main">
      <div class="subtabs__fields">
        <div class="subtabs__fields-top">
          <div class="subtabs__field">

            <h3 class="subtabs__field-title">{{ props.currentInnerTab.features[0].title }}</h3>
            <p class="subtabs__field-text">{{ props.currentInnerTab.features[0].content }}</p>
          </div>
          <div class="subtabs__field">
            <h3 class="subtabs__field-title">{{ props.currentInnerTab.features[2].title }}</h3>
            <p class="subtabs__field-text">{{ props.currentInnerTab.features[2].content }}</p>
          </div>
        </div>
        <div class="subtabs__stages">
          <div class="subtabs__stages-step">
            <div class="subtabs__stages-circle"></div>
          </div>
          <div class="subtabs__stages-line"></div>
          <div class="subtabs__stages-step">
            <div class="subtabs__stages-circle"></div>
          </div>
          <div class="subtabs__stages-line"></div>
          <div class="subtabs__stages-step">
            <div class="subtabs__stages-circle"></div>
          </div>
          <div class="subtabs__stages-line"></div>
          <div class="subtabs__stages-step">
            <div class="subtabs__stages-circle"></div>
          </div>
        </div>
        <div class="subtabs__fields-bottom">
          <div class="subtabs__field">
            <h3 class="subtabs__field-title">{{ props.currentInnerTab.features[1].title }}</h3>
            <p class="subtabs__field-text">{{ props.currentInnerTab.features[1].content }}</p>
          </div>
          <div class="subtabs__field">
            <h3 class="subtabs__field-title">{{ props.currentInnerTab.features[3].title }}</h3>
            <p class="subtabs__field-text">{{ props.currentInnerTab.features[3].content }}</p>
          </div>
        </div>
        <div class="subtabs__fields-line">
          <div class="subtabs__field-decor">
              <div class="subtabs__field-decor-circle"></div>
          </div>
          <div class="subtabs__field-decor">
              <div class="subtabs__field-decor-circle"></div>
          </div>
          <div class="subtabs__field-decor">
              <div class="subtabs__field-decor-circle"></div>
          </div>
          <div class="subtabs__field-decor">
              <div class="subtabs__field-decor-circle"></div>
          </div>
        </div>
      </div>
      <div class="subtabs__info">
        <h3 class="subtabs__title">{{ props.currentInnerTab.name }}</h3>
        <p class="subtabs__text">
          {{ props.currentInnerTab.desc }} 
        </p>
      </div>
    </div>
  </div>
</template>

<style>
/* Mobile menu  */



/* STYLES  */

.subtabs {
  min-height: 540px;
  border-radius: 20px;
  border: 1px solid var(--color-border);
  background: #FFF;
  padding: 30px;
  display: grid;
  grid-template-columns: 240px 1fr;
  gap: 82px;
}

.subtabs__nav {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 20px;
}

.subtabs__link {
  position: relative;
  border-radius: 10px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);
  padding: 21px 22px;

  color: #FFF;
  font-family: 'Inter', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 500;
  line-height: 13px;
  display: block;
  max-width: 234px;
}
.subtabs__link-icon {
  width: 46px;
  height: 46px;
  position: absolute;
  top: 50%;
  right: 5px;
  transform: translateY(-50%);
  border-radius: 8px;
  background: var(--color-tertiary);
  display: flex;
  justify-content: center;
  align-items: center;
}

.subtabs__menu {
  position: relative;
}

.subtabs__menu-btn {
  width: 100%;
  cursor: pointer;
  font-family: 'Inter', sans-serif;
  position: relative;
  border-radius: 40px;
  border: 1px solid var(--color-border);
  background: var(--color-btns);
  padding: 10px 40px;

  color: #FFF;
  text-align: center;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  display: none;
}

.subtabs__menu-icon {
  position: absolute;
  right: 5px;
  top: 50%;
  transform: translateY(-50%);
}

.subtabs__btn {
  position: relative;
  display: block;
  width: 100%;
  border-radius: 40px;
  border: 1px solid transparent;
  background: none;
  cursor: pointer;
  padding: 10px 20px;

  color: var(--color-btns);
  text-align: left;
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  transition: background-color 0.2s, color 0.5s;
}

.subtabs__btn + .subtabs__btn {
  margin-top: 10px;
}

.subtabs__btn-icon {
  position: absolute;
  top: 50%;
  right: 14px;
  transform: translateY(-50%);
}

.subtabs__btn:hover {
  background: var(--color-btns);
  color: #FFF;
  border: 1px solid var(--color-border);
}

.subtabs__btn.active {
  background: var(--color-btns);
  color: #FFF;
  border: 1px solid var(--color-border);
}

.subtabs__main {
  background: url('/tabs-decor.svg');
  background-size: 361px;
  background-position: top right;
  background-repeat: no-repeat;
}

.subtabs__fields {
  position: relative;
  padding-top: 70px;
  margin-bottom: 82px;
}

.subtabs__fields-line {
  position: absolute;
  z-index: 0;
  top: 0;
  left: 15px;
  background: var(--color-primary);
  width: 1px;
  height: 90%;
  display: none;
}

.subtabs__field-decor {
  position: absolute;
  top: 0px;
  left: -15px;
  width: 31px;
  height: 31px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.subtabs__field-decor:nth-child(2) {
  top: 30%;
}

.subtabs__field-decor:nth-child(3) {
  top: 55%;
}

.subtabs__field-decor:nth-child(4) {
  top: unset;
  bottom: -1px;
}

.subtabs__field-decor::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: #fff;
  z-index: -1;
}

.subtabs__field-decor::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: rgba(136, 146, 238, 0.3);
  z-index: 2;
}

.subtabs__field-decor-circle {
  width: 9px;
  height: 9px;
  border-radius: 50%;
  background-color: var(--color-primary);
}

.subtabs__fields-top {
  display: flex;
  align-items: center;
  gap: 100px;
}

.subtabs__fields-bottom {
  display: flex;
  align-items: center;
  gap: 100px;
  padding-left: 150px;
}

.subtabs__field {
  position: relative;
  border-radius: 10px;
  background: rgba(136, 146, 238, 0.30);
  backdrop-filter: blur(5px);
  padding: 10px 15px;
  max-width: 250px;
}

.subtabs__field-title {
  color: var(--color-btns);
  font-size: 13px;
  font-style: normal;
  font-weight: 600;
  line-height: 16px; 
  margin-bottom: 10px;
}

.subtabs__field-text {
  color: #575757;
  font-size: 11px;
  font-style: normal;
  font-weight: 500;
  line-height: 16px;
}



.subtabs__info {
  padding-left: 77px;
}
.subtabs__title {
  color: var(--color-btns);
  font-size: 15px;
  font-style: normal;
  font-weight: 600;
  line-height: 20px;
  margin-bottom: 10px;
}
.subtabs__text {
  color: #575757;
  font-size: 11px;
  font-style: normal;
  font-weight: 500;
  line-height: 22px;
  max-width: 675px;
}

.subtabs__stages {
  padding-left: 83px;
  margin: 2px 0;
  display: flex;
  align-items: center;
  gap: 4px;
}

.subtabs__stages-step {
  width: 32px;
  height: 32px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgba(136, 146, 238, 0.3);
  flex-shrink: 0;
}

.subtabs__stages-circle {
  border-radius: 50%;
  width: 9px;
  height: 9px;
  background-color: var(--color-primary);
}

.subtabs__stages-line {
  border-radius: 30px;
  background: var(--color-primary);
  height: 1px;
  flex-basis: 110px;
}

.subtabs__menu-icon.active {
  width: 20px;
  height: 20px;
  right: 10px;
  /* transform: translateY(-50%) rotate(180deg); */
}

.subtabs__list.active {
  opacity: 1;
  pointer-events: auto;
  transform: translateY(2px);
}

@media(max-width: 1200px) {
  .subtabs__info {
    padding-left: 0;
  }

  .subtabs {
    gap: 50px;
  }

  .subtabs__fields-top, .subtabs__fields-bottom {
    gap: 50px;
  }
}

@media(max-width: 992px) {
  .subtabs__link {
    display: none;
  }

  .subtabs__stages {
    display: none;
  }

  .subtabs {
    display: block;
  }

  .subtabs__list {
    border-radius: 20px;
    border: 1px solid var(--color-border);
    background: var(--color-btns);
  }

  .subtabs__btn-icon {
    display: none;
  }

  .subtabs__btn + .subtabs__btn {
    margin-top: 0px;
  }

  .subtabs__btn {
    border-radius: 0px;
    border: none;
    background: none;
    cursor: pointer;
    padding: 20px;

    color: #fff;
    text-align: center;

    transition: none;
  }

  .subtabs__btn:hover {
    background: none;
    border: none;
  }

  .subtabs__btn.active {
    background: none;
    border: none;
  }

  .subtabs__list {
    z-index: 3;
    width: 100%;
    opacity: 0;
    pointer-events: none;
    position: absolute;
    left: 0;
    top: 100%;
  }

  .subtabs__menu-btn {
    display: block;
  }

  .subtabs__fields {
    margin: 20px 0;
    padding-top: 0;
    padding-left: 42px;
  }

  .subtabs__fields-bottom {
    padding-left: 0;
  }

  .subtabs__fields-top, .subtabs__fields-bottom {
    flex-direction: column;
    gap: 10px;
  }

  .subtabs__fields-top {
    margin-bottom: 10px;
  }

  .subtabs__field {
    max-width: 100%;
    width: 100%;
  }

  .subtabs__fields-line {
    display: block;
  }

  .subtabs__main {
    background: none;
  }
}
</style>