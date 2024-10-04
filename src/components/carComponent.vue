<template>
  <ul>
    <li class="container" v-for="item in filteredData" :key="item.brand">
      <ion-button class="main-button" router-link="/tabs/tab3">
        <button class="carBtn" :value="item.url">
          <div class="image-container">
            <img
              class="car-image"
              :src="`/assets/scenes/${item.url}.png`"
              alt=""
            />
          </div>
          <div class="text-container">
            <h1 class="car-name">{{ item.name }}</h1>
            <h3 class="car-year">{{ item.year }}</h3>
          </div>
        </button>
      </ion-button>
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
  background: transparent;
  --ripple-color: transparent;
  --background-activated: transparent;
  text-decoration: none;
}

ion-button {
  --background: transparent;
  --border-radius: 0px;
  --padding-top: 0px;
  --padding-bottom: 0px;
  --padding-start: 0em;
  --padding-end: 0em;
  -webkit-margin-start: 0px;
  margin-inline-start: 0px;
  -webkit-margin-end: 0px;
  margin-inline-end: 0px;
  margin-top: 0px;
  margin-bottom: 0px;
  min-height: 0px;
  width: 100%;
  height: 18vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.main-button {
  --box-shadow: none;
}

.container {
  width: 90%;
  height: 18vh;
  display: flex;
  flex-direction: row;
  display: flex;
  flex-direction: row;
  background: transparent;
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

.image-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 18vh;
  height: 100%;
  border-radius: 40px;
  background-color: #49ade7;
}

.image-container .brand-svg {
  height: 100%;
  padding: 15%;
}

.image-container .car-image {
  width: 85%;
  height: 85%;
  object-fit: contain;
}

.text-container {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  width: calc(100% - 18vh);
  padding-left: 1rem;
}

.text-container h1 {
  margin: 0px;
  padding: 0px;
  font-family: suse;
  font-weight: 700;
  font-size: 2rem;
  color: #49ade7;
  text-align: start;
}

.text-container h3 {
  margin: 0px;
  padding: 0px;
  font-family: suse;
  font-weight: 700;
  font-size: 1.3rem;
  color: black;
}

main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  margin-top: 5.6rem;
  width: 100%;
  flex-wrap: wrap;
  gap: 1.5rem;
}

.title-svg {
  width: 30px;
  height: 30px;
}

app-car {
  width: 90%;
}
</style>

<script>
import { IonButton } from "@ionic/vue";
import jsonData from "./json/cars.json";
import { useRouter } from "vue-router";

export default {
  name: "carlist",

  components: { IonButton, useRouter },

  setup() {},

  data() {
    return {
      data: jsonData,
    };
  },

  computed: {
    filteredData() {
      return this.data.filter((value) => {
        return value.brand == localStorage.getItem("brandSel");
      });
    },
  },
};
</script>
