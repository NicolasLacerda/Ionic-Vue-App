<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <main>
        <div class="top-bar">
          <div class="menu-title">
            <a id="backBtn" v-on:click="clear"
              ><svg
                height="20px"
                width="20px"
                x="0"
                y="0"
                viewBox="0 0 64 64"
                style="enable-background: new 0 0 512 512"
                xml:space="preserve"
                fill-rule="evenodd"
              >
                <g>
                  <path
                    d="M47.83 55.172 24.66 32 47.83 8.828c1.56-1.561 1.56-4.095 0-5.656s-4.1-1.561-5.66 0l-26 26a4.003 4.003 0 0 0 0 5.656l26 26c1.56 1.561 4.1 1.561 5.66 0s1.56-4.095 0-5.656z"
                    fill="#ffffff"
                    opacity="1"
                    data-original="#000000"
                  ></path>
                </g>
              </svg>
            </a>

            <h1>Coches</h1>

            <svg
              x="0"
              y="0"
              viewBox="0 0 39.055 39.054"
              style="enable-background: new 0 0 512 512"
              xml:space="preserve"
              class="title-svg"
            >
              <g>
                <path
                  d="M38.831 14.26a1.005 1.005 0 0 0-.775-.369h-3.801c-.938-2.474-2.16-4.898-3.549-5.813-4.805-3.161-17.55-3.161-22.355 0-1.39.916-2.607 3.343-3.55 5.813H1a.997.997 0 0 0-.775.369.995.995 0 0 0-.204.834l.563 2.728a1 1 0 0 0 .979.797h1.126c-1.087 1.254-1.614 2.833-1.621 4.413-.007 1.952.734 3.716 2.089 4.964.015.013.03.022.044.035v3.817c0 .827.672 1.5 1.5 1.5h3.506c.828 0 1.5-.673 1.5-1.5v-1.534h19.641v1.534c0 .827.672 1.5 1.5 1.5h3.506c.826 0 1.5-.673 1.5-1.5v-3.742c1.438-1.317 2.125-3.129 2.134-4.938.006-1.634-.545-3.271-1.696-4.551h1.201a.996.996 0 0 0 .979-.798l.564-2.727a1.008 1.008 0 0 0-.205-.832zM9.998 10.583c3.83-2.521 15.229-2.521 19.057 0 .744.488 1.701 2.461 2.578 4.877H7.422c.875-2.415 1.832-4.387 2.576-4.877zM5.512 23.408a2.95 2.95 0 1 1 5.901.001 2.95 2.95 0 0 1-5.901-.001zm25.119 2.951a2.951 2.951 0 1 1 0-5.903 2.951 2.951 0 0 1 0 5.903z"
                  fill="#ffffff"
                  opacity="1"
                  data-original="#000000"
                  class=""
                ></path>
              </g>
            </svg>
          </div>
        </div>
        <carlist />
      </main>
    </ion-content>
  </ion-page>
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
}

main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  margin-top: 5.6rem;
  width: 100%;
  flex-wrap: wrap;
  margin-bottom: 1.2rem;
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
import { IonPage, IonContent, useBackButton, useIonRouter } from "@ionic/vue";
import carlist from "@/components/carComponent.vue";

export default {
  components: {
    IonPage,
    IonContent,
    useBackButton,
    useIonRouter,
    carlist,
  },

  setup() {
    useBackButton(9999, (processNextHandler) => {
      setTimeout(() => {
        let view = localStorage.getItem("view");
        setTimeout(() => {
          if (view == "true") {
            localStorage.removeItem("brandSel");
            location.href = "/tabs/tab1";
          } else {
            processNextHandler();
          }
        }, 10);
      }, 5);
    });

    setTimeout(() => {
      let allBtn = document.querySelectorAll(".carBtn");

      allBtn.forEach((bt) => {
        bt.addEventListener("click", (e) => {
          localStorage.setItem(
            "carName",
            bt.querySelectorAll(".car-name")[0].innerHTML
          );
        });
      });

      allBtn.forEach((bt) => {
        bt.addEventListener("click", (e) => {
          localStorage.setItem(
            "carYear",
            bt.querySelectorAll(".car-year")[0].innerHTML
          );
        });
      });

      allBtn.forEach((bt) => {
        bt.addEventListener("click", (e) => {
          localStorage.setItem("carUrl", bt.value);
        });
      });
    }, 25);
  },

  ionViewDidEnter() {
    localStorage.setItem("view", true);
  },

  ionViewDidLeave() {
    localStorage.setItem("view", false);
  },

  computed: {},

  methods: {
    clear: function () {
      localStorage.removeItem("brandSel");
      location.href = "/tabs/tab1";
    },
  },
};
</script>
