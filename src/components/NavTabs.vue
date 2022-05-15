<template>
  <ul class="nav nav-tabs mb-4">
    <li v-for="tab in tabs" :key="tab.id" class="nav-item">
      <router-link :to="tab.path" class="nav-link">
        {{ tab.title }}
      </router-link>
    </li>
    <!-- <li class="nav-item">
      <router-link to="/restaurants/feeds" class="nav-link">
        最新動態
      </router-link>
    </li>
    <li class="nav-item">
      <router-link to="/restaurants/top" class="nav-link">
        TOP 10 人氣餐廳
      </router-link>
    </li>
    <li class="nav-item">
      <router-link to="/users/top" class="nav-link"> 美食達人 </router-link>
    </li> -->
  </ul>
</template>

<script>
import { v4 as uuidv4 } from "uuid";

// const tabs=[] 這個無法往上代
const tabs = [
  {
    id: uuidv4(),
    title: "首頁",
    path: "/restaurants",
  },
  {
    id: uuidv4(),
    title: "最新動態",
    path: "/restaurants/feeds",
  },
  {
    id: uuidv4(),
    title: "TOP 10 人氣餐廳",
    path: "/restaurants/top",
  },
  {
    id: uuidv4(),
    title: "美食達人",
    path: "/users/top",
  },
];
export default {
  data() {
    return {
      tabs,
    };
  },
};
</script>