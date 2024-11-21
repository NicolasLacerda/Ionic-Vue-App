<template>
  <ion-page>
    <ion-content :fullscreen="true">
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
      <main>
        <carlist />
      </main>
      <ion-button class="help-btn" router-link="/tabs/tab8">
        <button href="/tabs/tab8">
          <svg
            x="0"
            y="0"
            viewBox="0 0 24 24"
            style="enable-background: new 0 0 512 512"
            xml:space="preserve"
            class="help-icon"
          >
            <g>
              <g fill="#000">
                <path
                  d="M7.25 8A.75.75 0 0 1 8 7.25h4a.75.75 0 0 1 0 1.5H8A.75.75 0 0 1 7.25 8zM7.25 12a.75.75 0 0 1 .75-.75h8a.75.75 0 0 1 0 1.5H8a.75.75 0 0 1-.75-.75z"
                  fill="#ffffff"
                  opacity="1"
                  data-original="#000000"
                  class=""
                ></path>
                <path
                  fill-rule="evenodd"
                  d="M9.966 1.25h4.068c1.371 0 2.447 0 3.311.07.88.073 1.607.221 2.265.557a5.75 5.75 0 0 1 2.513 2.513c.336.658.484 1.385.556 2.265.071.864.071 1.94.071 3.311v1.365c0 1.549 0 2.493-.232 3.287a5.75 5.75 0 0 1-3.9 3.9c-.794.232-1.738.232-3.287.232h-.756a4.25 4.25 0 0 0-2.42.776l-.05.035-2.61 1.865C7.99 22.5 6.012 20.948 6.7 19.232a.351.351 0 0 0-.327-.482h-.601a4.522 4.522 0 0 1-4.522-4.522V9.966c0-1.371 0-2.447.07-3.311.073-.88.221-1.607.557-2.265A5.75 5.75 0 0 1 4.39 1.877c.658-.336 1.385-.484 2.265-.556.864-.071 1.94-.071 3.311-.071zM6.777 2.816c-.787.064-1.295.188-1.706.397a4.25 4.25 0 0 0-1.858 1.858c-.21.411-.333.919-.397 1.706-.065.796-.066 1.81-.066 3.223v4.228a3.022 3.022 0 0 0 3.022 3.022h.601a1.851 1.851 0 0 1 1.72 2.539c-.131.326.244.62.53.416L11.29 18.3a5.75 5.75 0 0 1 3.276-1.05H15.184c1.742 0 2.452-.008 3.012-.172a4.25 4.25 0 0 0 2.882-2.882c.164-.56.172-1.27.172-3.012V10c0-1.413 0-2.427-.066-3.223-.064-.787-.188-1.295-.397-1.706a4.25 4.25 0 0 0-1.857-1.858c-.412-.21-.92-.333-1.707-.397-.796-.065-1.81-.066-3.223-.066h-4c-1.413 0-2.427 0-3.223.066z"
                  clip-rule="evenodd"
                  fill="#ffffff"
                  opacity="1"
                  data-original="#000000"
                  class=""
                ></path>
              </g>
            </g>
          </svg>
        </button>
      </ion-button>
    </ion-content>
  </ion-page>
</template>

<style scoped>
.help-btn {
  width: 4rem;
  height: 4rem;
  position: fixed;
  bottom: 1.35rem;
  right: 1.35rem;
  display: flex;
  justify-content: center;
  align-items: center;
  --box-shadow: none;
}

.help-btn button {
  width: 4rem;
  height: 4rem;
  background-color: #49ade7;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
}

.help-btn .help-icon {
  width: 2.35rem;
  height: 2.35rem;
}

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
import {
  IonPage,
  IonContent,
  useBackButton,
  useIonRouter,
  IonButton,
} from "@ionic/vue";
import carlist from "@/components/carComponent.vue";

export default {
  components: {
    IonPage,
    IonContent,
    useBackButton,
    useIonRouter,
    carlist,
    IonButton,
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
