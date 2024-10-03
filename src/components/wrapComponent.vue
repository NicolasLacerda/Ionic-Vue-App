<template>
  <ul>
    <li class="container" v-for="item in filteredData" :key="item.brand">
      <button class="wrapBtn" :value="item.model">
        <router-link to="/tabs/tab5">
          <div class="image-container">
            <img
              class="wrap-image"
              :src="`/assets/img/wrapTypes/${item.image}`"
              alt=""
            />
          </div>
          <div class="text-container">
            <h1 class="wrap-name">{{ item.name }}</h1>
            <h3 class="wrap-model">{{ item.model }}</h3>
            <h3 class="hideVinils">{{ item.vinils }}</h3>
          </div>
        </router-link>
      </button>
    </li>
  </ul>
</template>

<style scoped>
ul {
  margin-block-start: 0 !important;
  margin-block-end: 0 !important;
  padding-inline-start: 0 !important;
  gap: 1.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}

.container a {
  display: flex;
  flex-direction: row;
  text-decoration: none;
  width: 100%;
  height: 100%;
}

.container {
  width: 90%;
  height: 18vh;
  display: flex;
  flex-direction: row;
  display: flex;
  flex-direction: row;
  background: transparent;
  --ripple-color: transparent;
  --background-activated: transparent;
  text-decoration: none;
}

button {
  display: flex;
  flex-direction: row;
  background: transparent;
  color: black;
  width: 100%;
  height: 18vh;
  justify-content: center;
  align-items: center;
}

ion-tab-button {
  display: flex;
  flex-direction: row;
}

.image-container {
  display: flex;
  justify-content: center;
  align-items: end;
  width: 18vh;
  height: 100%;
  border-radius: 40px;
  background-color: #49ade7;
}

.image-container .wrap-image {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.text-container {
  height: 100%;
  display: flex;
  flex-direction: column-reverse;
  justify-content: center;
  align-items: flex-start;
  width: calc(100% - 18vh);
  padding-left: 1rem;
}

.text-container h3 {
  margin: 0px;
  padding: 0px;
  font-family: suse;
  font-weight: 700;
  font-size: 1.5rem;
  color: #49ade7;
  text-transform: capitalize;
}

.text-container h1 {
  margin: 0px;
  padding: 0px;
  font-family: suse;
  font-weight: 700;
  font-size: 1.3rem;
  text-align: start;
  color: black;
}

.hideVinils {
  width: 0px;
  height: 0px;
  font-size: 0px !important;
}
</style>

<script>
import jsonData from "./json/wrap.json";

export default {
  name: "wraplist",

  components: {},

  setup() {},

  data() {
    return {
      data: jsonData,
    };
  },

  computed: {
    filteredData() {
      return this.data.filter((value) => {
        return value.brand == localStorage.getItem("brandWrapSel");
      });
    },
  },
};
</script>
