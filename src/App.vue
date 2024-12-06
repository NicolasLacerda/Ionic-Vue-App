<script setup lang="ts">
import { IonApp, IonRouterOutlet } from "@ionic/vue";
</script>

<template>
  <ion-app>
    <ion-router-outlet />
  </ion-app>
</template>

<style>
@font-face {
  font-family: suse;
  src: url(https://brazwrap.es/wp-content/uploads/assets/fonts/suse.ttf);
}

ion-button {
  --ripple-color: transparent !important;
  --color-hover: transparent !important;
  --background-hover: transparent !important;
}

ion-button:active {
  --ripple-color: transparent !important;
  --color-hover: transparent !important;
  --background-hover: transparent !important;
}

h1 {
  margin: 0px;
}

.header-md {
  -webkit-box-shadow: none;
  box-shadow: none;
}

ion-content {
  background-color: rgb(253, 253, 253) !important;
  --offset-bottom: auto !important;
  --overflow: hidden;
  overflow: auto;
  &::-webkit-scrollbar {
    display: none;
  }
}

ion-tab-button {
  max-width: inherit;
  --padding-start: 0px;
  --padding-end: 0px;
  position: initial;
  display: flex;
  flex-direction: row;
  background: transparent;
  --ripple-color: transparent;
  --background-activated: transparent;
}

.top-bar {
  background: #0089c1;
  height: 4.4rem;
  width: 100%;
  border-radius: 0px 0px 30px 30px;
  position: fixed;
  top: 0;
  z-index: 99;
}

.menu-title {
  padding-top: 1.5rem;
  padding-bottom: 0.5rem;
  margin-left: auto;
  margin-right: auto;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  width: calc(90% - 1rem);
  height: 100%;
}

.menu-title h1 {
  font-family: suse;
  font-weight: 700;
  font-size: 1.9rem;
  color: white;
  margin-top: 0.8rem;
}

.title-svg {
  height: 1.7rem;
}

ion-content {
  background: white;
}
</style>
