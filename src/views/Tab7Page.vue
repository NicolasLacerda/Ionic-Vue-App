<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div class="top-bar">
        <div class="menu-title">
          <a id="back-btn-config" v-on:click="clear"
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

          <h1 class="title">configurações</h1>

          <div class="title-svg"></div>
        </div>
      </div>
      <main>
        <div class="config-content">
          <div class="content-inner">
            <div class="icon_and_title">
              <svg
                x="0"
                y="0"
                viewBox="0 0 24 24"
                style="enable-background: new 0 0 512 512"
                xml:space="preserve"
                class="menu-svg"
              >
                <g>
                  <path
                    d="m22.683 9.394-1.88-.239a9.45 9.45 0 0 0-.569-1.374l1.161-1.495a1.486 1.486 0 0 0-.122-1.979l-1.575-1.575a1.49 1.49 0 0 0-1.985-.127L16.22 3.766a9.416 9.416 0 0 0-1.375-.569l-.239-1.877A1.498 1.498 0 0 0 13.12 0h-2.24c-.757 0-1.396.567-1.486 1.317l-.239 1.88a9.307 9.307 0 0 0-1.375.569L6.286 2.605a1.488 1.488 0 0 0-1.979.122L2.732 4.301a1.49 1.49 0 0 0-.127 1.986l1.161 1.494a9.34 9.34 0 0 0-.569 1.374l-1.877.239C.567 9.484 0 10.123 0 10.88v2.24c0 .757.567 1.396 1.317 1.486l1.88.239c.155.477.346.937.569 1.374l-1.161 1.495a1.486 1.486 0 0 0 .122 1.979l1.575 1.575a1.492 1.492 0 0 0 1.985.126l1.494-1.161c.437.224.897.415 1.374.569l.239 1.876c.09.755.729 1.322 1.486 1.322h2.24c.757 0 1.396-.567 1.486-1.317l.239-1.88a9.45 9.45 0 0 0 1.374-.569l1.495 1.161c.605.47 1.459.415 1.979-.122l1.575-1.575a1.49 1.49 0 0 0 .127-1.985l-1.161-1.494c.224-.437.415-.897.569-1.374l1.876-.239a1.498 1.498 0 0 0 1.32-1.486v-2.24a1.496 1.496 0 0 0-1.316-1.486zM12 17c-2.757 0-5-2.243-5-5s2.243-5 5-5 5 2.243 5 5-2.243 5-5 5z"
                    fill="#49ade7"
                    opacity="1"
                    data-original="#000000"
                    class=""
                  ></path>
                </g>
              </svg>
              <p class="quality">Qualidade Gráfica</p>
            </div>
            <div class="buttons-container">
              <button class="btG b1" value="high">Alto</button>
              <button class="btG b2" value="medium">Médio</button
              ><button class="btG b3" value="low">Baixo</button>
            </div>
          </div>
          <p class="information">
            O Anti Serrilhado quando está ligado pode gerar travamentos e
            congelamentos. Caso tiver um aparelho mais fraco melhor deixa-lo
            desligado.
          </p>
        </div>
      </main>
    </ion-content>
  </ion-page>
</template>

<style scoped>
.menu-svg {
  width: 6.5rem;
}

.icon_and_title {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 1rem;
}

.title {
  position: absolute;
  z-index: 1;
  left: 50%;
  transform: translate(-50%, -20%);
}

main {
  background: white;
  background-position: center center;
  background-size: cover;
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
}

.config-content {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 100%;
  margin-top: 4.4rem;
}

.content-inner {
  height: 100%;
  width: 80%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 2.5rem;
}

.quality {
  width: 90%;
  font-size: 1.4rem;
  color: #49ade7;
  margin: 0px;
  border-radius: 20px;
  font-weight: 700;
  text-align: center;
}

.buttons-container {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}

#callAlias {
  width: 80%;
}

.buttons-container button {
  padding: 1rem;
  width: 45%;
  background-color: #49ade7;
  color: white;
  font-size: 1.4rem;
  font-weight: 700;
  border-radius: 500px;
}

.buttons-container button:nth-child(2) {
  padding: 1rem;
  width: 50%;
  background-color: #49ade7;
  color: white;
  font-size: 1.4rem;
  font-weight: 700;
  border-radius: 500px;
}

.buttons-container button:nth-child(3) {
  padding: 1rem;
  width: 55%;
  background-color: #49ade7;
  color: white;
  font-size: 1.4rem;
  font-weight: 700;
  border-radius: 500px;
}

.information {
  width: 80%;
  background-color: #49ade7;
  color: white;
  font-weight: 600;
  padding: 1rem;
  border-radius: 20px;
  text-align: center;
}
</style>

<script>
import {
  IonPage,
  IonContent,
  IonButton,
  useBackButton,
  useIonRouter,
} from "@ionic/vue";
import { useRouter } from "vue-router";

export default {
  components: {
    IonPage,
    IonContent,
    IonButton,
    useRouter,
    useBackButton,
    useIonRouter,
  },

  setup() {
    useBackButton(9999, (processNextHandler) => {
      setTimeout(() => {
        let view = localStorage.getItem("view");
        setTimeout(() => {
          if (view == "true") {
            history.back();
          } else {
            processNextHandler();
          }
        }, 10);
      }, 5);
    });

    setTimeout(() => {
      let b1, b2, b3;

      b1 = document.querySelector(".b1");
      b2 = document.querySelector(".b2");
      b3 = document.querySelector(".b3");

      b1.addEventListener("click", (e) => {
        localStorage.setItem("graphic", "high");
        localStorage.setItem("shadow", true);
        localStorage.setItem("alias", true);
        localStorage.setItem("renderH", 1280);
        localStorage.setItem("renderW", 720);
        localStorage.setItem("model", "assets/scenes/");
        location.reload();
      });

      b2.addEventListener("click", (e) => {
        localStorage.setItem("graphic", "medium");
        localStorage.setItem("shadow", false);
        localStorage.setItem("alias", true);
        localStorage.setItem("renderH", 1024);
        localStorage.setItem("renderW", 768);
        localStorage.setItem("model", "assets/scenes/");
        location.reload();
      });

      b3.addEventListener("click", (e) => {
        localStorage.setItem("graphic", "low");
        localStorage.setItem("shadow", false);
        localStorage.setItem("alias", false);
        localStorage.setItem("renderH", 800);
        localStorage.setItem("renderW", 600);
        localStorage.setItem("model", "assets/scenes/low/");
        location.reload();
      });

      if (localStorage.getItem("graphic") == "medium") {
        b2.style.color = "#49ade7";
        b2.style.background = "white";
        b2.style.border = "#49ade7 2px solid";
      } else if (localStorage.getItem("graphic") == "low") {
        b3.style.color = "#49ade7";
        b3.style.background = "white";
        b3.style.border = "#49ade7 2px solid";
      } else {
        b1.style.color = "#49ade7";
        b1.style.background = "white";
        b1.style.border = "#49ade7 2px solid";
      }
    }, 5);
  },

  ionViewDidEnter() {
    localStorage.setItem("view", true);
  },

  ionViewDidLeave() {
    localStorage.setItem("view", false);
  },

  methods: {
    clear: function () {
      history.back();
    },
  },
};
</script>
