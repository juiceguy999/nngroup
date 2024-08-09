<script setup>
import SubTabs from './SubTabs.vue'
import { ref, onMounted } from 'vue'

// onMounted(async () => {
//   const {data: casesData} = await axios.request({
//     withCredentials: true,
//     headers: {
//       Authorization: `Bearer ${bearerToken}`
//     },
//     method: "GET",
//     url: `/api/cases`
//   });

//   casesData.forEach(caseObj => {
//     data.value.forEach(dataObj => {
//       if(caseObj.type !== dataObj.type) return;
//       dataObj.cases.push(caseObj);
//     })
//   });

//   currentInnerTab.value = currentTab.value.cases[0];
// })

const data = ref(null);

const currentTab = ref(null);
const currentInnerTab = ref(null);

onMounted(async () => {
  const res = await fetch('/api/cases');
  const resData = await res.json();
  data.value = resData;
  
  currentTab.value = data.value?.[0];
  currentInnerTab.value = currentTab.value?.cases?.[0]
})


const handleTab = (tab) => {
  currentTab.value = tab;
  currentInnerTab.value = tab.cases[0];
}

const handleChangeTab = (subtab) => {
  currentInnerTab.value = subtab;
}



</script>

<template>
  <div class="tabs" v-if="currentInnerTab">
    <h2 class="tabs__title">Мы способны на ВСЁ!</h2>
    <div class="tabs__btns">
      <button v-for="tab in data" :key="JSON.stringify(tab)" :class="['tabs__btn', { active: currentTab === tab }]"
        @click="handleTab(tab)">
        {{tab.name}}
      </button>
    </div>
    <SubTabs @changeTab="handleChangeTab" :currentInnerTab="currentInnerTab" :currentTab="currentTab" />
  </div>

</template>

<style scoped>
.tabs__title {
  color: var(--color-btns);
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 60px;
  text-transform: uppercase;
  margin-bottom: 40px;
}
.tabs__btns {
  display: flex;
  align-items: center;
  gap: 10px;
  border-radius: 20px;
  border: 1px solid var(--color-border);
  padding: 5px 6px;
  margin-bottom: 30px;
}

.tabs__btn {
  border: none;
  background: transparent;
  cursor: pointer;
  border-radius: 16px;
  padding: 15px 30px;
  height: 50px;

  color: rgba(25, 25, 25, 0.50);
  text-align: center;
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
  transition: background-color 0.2s, color 0.5s;
}

.tabs__btn:hover {
  background: var(--color-btns);
  color: #FFF;
}

.tabs__btn.active {
  background: var(--color-btns);
  color: #FFF;
}

@media(max-width: 1200px) {
  .tabs__btn {
    padding: 10px 20px;
    font-size: 12px;
    font-style: normal;
    font-weight: 500;
    line-height: 20px; /* 166.667% */
    border-radius: 20px;
  }
}

@media(max-width: 992px) {
  .tabs__btns {
    border: none;
    flex-wrap: wrap;
    padding: 0;
  }

  .tabs__btn {
    color: var(--color-btns);
    border-radius: 100px;
    border: 1px solid var(--color-border);
    background: rgba(255, 255, 255, 0.01);
    backdrop-filter: blur(5px);
  }

  .tabs__title {
    font-size: 30px;
    font-style: normal;
    font-weight: 700;
    line-height: 60px;
    text-transform: uppercase;
    margin-bottom: 20px;
  }
}

@media(max-width: 576px) {
  .tabs__title {
    font-size: 26px;
  }
}
</style>