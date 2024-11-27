<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div class="top-bar">
        <div class="menu-title">
          <a id="back-btn-menu" v-on:click="clear"
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

          <h1 class="title">Detalhes</h1>
        </div>
      </div>
      <main>
        <div class="menu-page">
          <div class="menu-page-inner">
            <div class="carInfo">
              <div class="carImg"></div>
              <h3 class="carName"></h3>
            </div>

            <div class="moreInfos">
              <div class="moreInfos-inner">
                <div class="blocks">
                  <div class="icons-circle">
                    <svg
                      x="0"
                      y="0"
                      viewBox="0 0 25.954 25.954"
                      style="enable-background: new 0 0 512 512"
                      xml:space="preserve"
                      class="infoIcons"
                    >
                      <g transform="matrix(-1,0,0,1,25.954514938406646,0)">
                        <path
                          d="M24.44 5.994C15.143 5.994 18.172 0 11.505 0 7.286 0 6.518 2.148 5.846 4.166 5.253 5.945.467 18.511.467 18.511l.035-.048C.17 19.158.003 19.87.003 20.51c0 2.705 1.889 5.444 5.5 5.444 4.055 0 5.5-2.066 5.5-4 0-2.289-2.386-4-4.519-4-2.405 0-3.481 1.256-3.481 2.5 0 1.425 1.29 2.5 3 2.5a1 1 0 1 0 0-2c-.533 0-1-.233-1-.5 0-.204.527-.5 1.481-.5 1.11 0 2.519.941 2.519 2 0 1.74-2.193 2-3.5 2-2.418 0-3.5-1.729-3.5-3.444 0-.923.871-3.556 4.74-3.556 3.107 0 4.196 1.617 5.574 3.664 1.6 2.377 3.591 5.336 9.294 5.336.513 0 .919-.39.977-.887h.012s3.096-16.54 3.277-17.332c.47-2.047-1.437-1.741-1.437-1.741z"
                          data-original="#030104"
                          class=""
                          opacity="1"
                        ></path>
                      </g>
                    </svg>
                  </div>
                  <p class="brand"></p>
                </div>
                <div class="blocks">
                  <div class="icons-circle">
                    <svg
                      x="0"
                      y="0"
                      viewBox="0 0 64 64"
                      style="enable-background: new 0 0 512 512"
                      xml:space="preserve"
                      class="infoIcons"
                    >
                      <g
                        transform="matrix(1.0799999999999998,0,0,1.0799999999999998,-2.559999999999995,-1.4561700439453062)"
                      >
                        <path
                          d="M18.41 13c4.05 0 8.4-1.12 8.4-3.58-.11-4.789-16.7-4.783-16.81 0 0 2.46 4.36 3.58 8.41 3.58zm0-5.15c4.11 0 6.28 1.15 6.41 1.56-.13.44-2.3 1.59-6.41 1.59-4.07 0-6.23-1.13-6.41-1.58.18-.45 2.34-1.57 6.41-1.57z"
                          opacity="1"
                          data-original="#000000"
                          class=""
                        ></path>
                        <path
                          d="M56 14.56H32.813V9.343C32.393-.205 4.405-.198 4 9.34a3.863 3.863 0 0 1 0 1.33v42.66c0 3.83 7.42 5.89 14.4 5.89H56a4.005 4.005 0 0 0 4-4V18.56a3.999 3.999 0 0 0-4-4zM29.14 46.37l10.17-22.01a1.003 1.003 0 0 1 1.82.84L30.96 47.21a1.002 1.002 0 0 1-1.82-.84zm-8.23.84a1.002 1.002 0 0 1-1.82-.84l10.18-22.01a.998.998 0 0 1 1.81.84zM51.18 25.2 41.01 47.21a1.002 1.002 0 0 1-1.82-.84l10.17-22.01a1.003 1.003 0 0 1 1.82.84zM28.45 14.56a10.837 10.837 0 0 0 2.363-1.503v1.503zM18.41 4.13c7.31 0 12.4 2.75 12.4 5.21 0 2.47-5.09 5.22-12.4 5.22S6 11.81 6 9.34c0-2.46 5.1-5.21 12.41-5.21z"
                          opacity="1"
                          data-original="#000000"
                          class=""
                        ></path>
                      </g>
                    </svg>
                  </div>
                  <p class="type"></p>
                </div>
              </div>
              <div class="moreInfos-inner">
                <div class="block">
                  <div class="blocks">
                    <div class="icons-circle">
                      <svg
                        x="0"
                        y="0"
                        viewBox="0 0 512 512"
                        style="enable-background: new 0 0 512 512"
                        xml:space="preserve"
                        class="infoIcons"
                      >
                        <g>
                          <path
                            d="M494.26 276.22c-3.6-40.41-9.53-48.28-11.77-51.24-5.15-6.84-13.39-11.31-22.11-16a3.6 3.6 0 0 1-.91-5.68 15.93 15.93 0 0 0 4.53-12.53A16.27 16.27 0 0 0 447.65 176h-15.6a17 17 0 0 0-2 .13 8.5 8.5 0 0 0-1.41-.47c-9.24-19.53-21.89-46.27-48.11-59.32C341.64 97 270 96 256 96s-85.64 1-124.48 20.31c-26.22 13.05-38.87 39.79-48.11 59.32l-.08.16a6.52 6.52 0 0 0-1.35.34 17 17 0 0 0-2-.13H64.35A16.27 16.27 0 0 0 48 190.77a15.93 15.93 0 0 0 4.59 12.47 3.6 3.6 0 0 1-.91 5.68c-8.72 4.72-17 9.19-22.11 16-2.24 3-8.16 10.83-11.77 51.24-2 22.74-2.3 46.28-.73 61.44 3.29 31.5 9.46 50.54 9.72 51.33a16 16 0 0 0 13.2 10.87v.2a16 16 0 0 0 16 16h56a16 16 0 0 0 16-16c8.61 0 14.6-1.54 20.95-3.18a158.83 158.83 0 0 1 28-4.91C207.45 389 237.79 388 256 388c17.84 0 49.52 1 80.08 3.91a159.16 159.16 0 0 1 28.11 4.93c6.08 1.56 11.85 3 19.84 3.15a16 16 0 0 0 16 16h56a16 16 0 0 0 16-16v-.12A16 16 0 0 0 485.27 389c.26-.79 6.43-19.83 9.72-51.33 1.57-15.17 1.29-38.67-.73-61.45zm-381.93-86.91c8-17 17.15-36.24 33.44-44.35 23.54-11.72 72.33-17 110.23-17s86.69 5.24 110.23 17c16.29 8.11 25.4 27.36 33.44 44.35l1 2.17a8 8 0 0 1-7.44 11.42C360 202 290 199.12 256 199.12s-104 2.95-137.28 3.85a8 8 0 0 1-7.44-11.42c.35-.74.72-1.49 1.05-2.24zm11.93 79.63A427.17 427.17 0 0 1 72.42 272c-10.6 0-21.53-3-23.56-12.44-1.39-6.35-1.24-9.92-.49-13.51C49 243 50 240.78 55 240c13-2 20.27.51 41.55 6.78 14.11 4.15 24.29 9.68 30.09 14.06 2.91 2.16 1.36 7.8-2.38 8.1zm221.38 82c-13.16 1.5-39.48.95-89.34.95s-76.17.55-89.33-.95c-13.58-1.51-30.89-14.35-19.07-25.79 7.87-7.54 26.23-13.18 50.68-16.35s34.8-4.8 57.62-4.8 32.12 1 57.62 4.81 44.77 9.52 50.68 16.35c10.78 12.24-5.29 24.19-18.86 25.84zm117.5-91.39c-2 9.48-13 12.44-23.56 12.44a455.91 455.91 0 0 1-52.84-3.06c-3.06-.29-4.48-5.66-1.38-8.1 5.71-4.49 16-9.91 30.09-14.06 21.28-6.27 33.55-8.78 44.09-6.69 2.57.51 3.93 3.27 4.09 5a40.64 40.64 0 0 1-.49 14.48z"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                        </g>
                      </svg>
                    </div>
                    <p class="infoColor"></p>
                  </div>
                  <div class="blocks">
                    <div class="icons-circle">
                      <svg
                        style="
                          shape-rendering: geometricPrecision;
                          text-rendering: geometricPrecision;
                          image-rendering: optimizeQuality;
                          fill-rule: evenodd;
                          clip-rule: evenodd;
                        "
                        viewBox="0 0 356.96 713.92"
                        class="infoIcons roof"
                      >
                        <g>
                          <path
                            class="fil0"
                            d="M76.69 584.25c0,-31.85 -7.18,-73.91 25.1,-73.91l153.38 0c32.28,0 25.1,42.06 25.1,73.91 0,22.09 -22.25,27.14 -39.32,31.79 -41.4,11.29 -83.54,11.29 -124.94,0 -16.84,-4.59 -39.32,-9.59 -39.32,-31.79zm230.07 -86.46l0 -103.18c0,-15.07 23.71,-15.07 23.71,0l0 103.18c0,15.07 -23.71,15.07 -23.71,0zm-280.27 0l0 -103.18c0,-15.07 23.71,-15.07 23.71,0l0 103.18c0,15.07 -23.71,15.07 -23.71,0zm0 -235.65c0,-15.21 4.65,-25.18 21.24,-28.95 73.64,-16.73 150.72,-22.24 225.93,-7.66 34.98,6.77 56.81,6.15 56.81,36.61 0,9.53 -36.94,88.25 -42.29,99.94 -5.3,11.59 -11.11,19.98 -27.43,19.98l-164.54 0c-25.13,0 -29.11,-24.6 -41.85,-52.96 -4.81,-10.69 -10.04,-21.4 -14.73,-32.69 -3.44,-8.29 -13.14,-26.42 -13.14,-34.27zm178.48 -211.94c0,-12.07 20.18,-19.01 24.55,1.94l24.82 125.18c0.23,7.98 -5.55,13.71 -11.72,13.71 -13.37,0 -13.73,-16.36 -16.15,-28.47l-14.87 -74.37c-1.96,-9.79 -6.63,-27.02 -6.63,-37.99zm-89.24 140.83c-19.76,0 -11.53,-22.52 -9.64,-31.95l16.96 -84.83c1.29,-6.42 2.68,-13.54 4.16,-20.95 4.6,-23.12 24.78,-14.15 24.78,-3.1 0,10.91 -4.23,26.01 -6.39,36.83l-14.88 74.37c-1.97,9.86 -3.19,29.63 -14.99,29.63zm-13.94 -181.27c0,24.89 -12.18,44.71 -27.28,54.99 -19.76,13.46 -40.03,11.94 -71.72,11.94 -1.55,6.64 -2.79,12.64 -2.79,20.92l0 507.55c0,21.09 9.15,44.56 20.69,60.18 20.55,27.82 51.44,48.58 88.07,48.58l139.44 0c32.45,0 69.63,-21.09 87.6,-47.65 3.33,-4.93 7.97,-11.84 10.44,-17.45 5.13,-11.7 10.72,-27.6 10.72,-43.66l0 -507.55c0,-8.28 -1.24,-14.28 -2.79,-20.92 -31.43,0 -51.08,1.5 -70.88,-11.38 -22.93,-14.91 -28.12,-36.2 -28.12,-65.31l-153.38 0 0 9.76z"
                          />
                          <path
                            class="fil0"
                            d="M50.2 257.96c0.96,4.12 2.87,7.42 4.77,11.96 2.11,5.04 3.36,7.22 5.58,12.55l27.32 61.92c1.71,3.81 3.71,8.73 5.55,12.57l170.12 0 38.05 -86.05c1.79,-4.14 4.29,-9.15 5.17,-12.95 -30.73,-7.16 -60.24,-12.52 -93.49,-15.26 -5.78,-0.48 -12.25,0.24 -18.06,-0.07 -25.78,-1.39 -7.68,-1.39 -33.45,0 -5.82,0.31 -12.29,-0.41 -18.07,0.07 -32.95,2.71 -62.86,8.13 -93.49,15.26z"
                          />
                          <path
                            class="fil0"
                            d="M101.79 585.64l33.73 9.5c25.97,6.13 58.88,5.64 84.95,0.41 13.44,-2.69 22.99,-7.18 34.7,-9.91l0 -50.2 -153.38 0 0 50.2z"
                          />
                          <path
                            class="fil0"
                            d="M13.94 51.59c21.2,0 35.38,1.74 47.66,-8.12 14.98,-12.04 15.09,-23.61 15.09,-40.68 -13.88,3.23 -26.29,10.34 -37.25,18.52 -8.21,6.12 -23.15,20.21 -25.5,30.28z"
                          />
                          <path
                            class="fil0"
                            d="M343.02 51.59c-1.2,-5.12 -7.63,-12.85 -10.94,-16.95 -10.79,-13.38 -34.55,-27.83 -51.81,-31.85 0,17.07 0.11,28.64 15.09,40.68 12.28,9.86 26.46,8.12 47.66,8.12z"
                          />
                        </g>
                      </svg>
                    </div>
                    <p class="roofColor"></p>
                  </div>
                </div>
                <div class="block">
                  <div class="blocks">
                    <div class="icons-circle">
                      <svg
                        x="0"
                        y="0"
                        viewBox="0 0 469.333 469"
                        style="enable-background: new 0 0 512 512"
                        xml:space="preserve"
                        class="infoIcons"
                      >
                        <g transform="matrix(1,0,0,1,0,70)">
                          <path
                            d="M298.668 64.168h-128C111.785 64.234 64.07 111.953 64 170.832V181.5c.012 5.887 4.781 10.656 10.668 10.668h224c11.777-.008 21.324-9.555 21.332-21.336V85.5c-.008-11.777-9.555-21.324-21.332-21.332zm0 0"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                          <path
                            d="M384 181.5V74.832C383.95 33.617 350.55.215 309.332.168H160C71.676.262.098 71.84 0 160.168v42.664c.027 29.445 23.89 53.309 53.332 53.336h256c41.219-.05 74.617-33.453 74.668-74.668zm-42.668-10.668c-.027 23.555-19.113 42.637-42.664 42.668h-224c-17.668-.02-31.98-14.336-32-32v-10.668c.074-70.66 57.34-127.922 128-128h128c23.55.031 42.637 19.117 42.664 42.668zm0 0"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                          <path
                            d="M458.668 64.168h-21.336a10.65 10.65 0 0 0-7.543 3.121c-2 2-3.125 4.715-3.121 7.543 0 27.606-8.871 34.008-21.336 39.457V181.5a95.709 95.709 0 0 1-46.652 81.914 109.479 109.479 0 0 1 68.527 70.793 10.689 10.689 0 0 0 10.125 7.293h21.336c2.828 0 5.543-1.121 7.543-3.121a10.66 10.66 0 0 0 3.121-7.547v-256c.004-2.828-1.121-5.543-3.121-7.543s-4.715-3.125-7.543-3.121zm0 0"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                        </g>
                      </svg>
                    </div>
                    <p class="retroColor"></p>
                  </div>
                  <div class="blocks">
                    <div class="icons-circle">
                      <svg
                        x="0"
                        y="0"
                        viewBox="0 0 60 60"
                        style="enable-background: new 0 0 512 512"
                        xml:space="preserve"
                        class="infoIcons"
                      >
                        <g
                          transform="matrix(-1,1.2246467991473532e-16,-1.2246467991473532e-16,-1,60.00001096725465,59.99849414825439)"
                        >
                          <path
                            d="M31 39a1 1 0 0 0 1-1V11.052c-.658-.028-1.319-.052-2-.052s-1.342.024-2 .052V38a1 1 0 0 0 1 1Z"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                          <path
                            d="M34 11.183V38a3 3 0 0 1-3 3h-2a3 3 0 0 1-3-3V11.183a45.632 45.632 0 0 0-12.2 2.743c-1.491 3.976-4.621 14.7-5.616 36.387C11.83 47.2 18.812 43 30 43s18.17 4.2 21.818 7.312C50.823 28.621 47.693 17.9 46.2 13.926A45.632 45.632 0 0 0 34 11.183Z"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                          <path
                            d="M50.565 11.66a47.7 47.7 0 0 0-41.133 0 6.924 6.924 0 0 0-3.5 3.837A46.868 46.868 0 0 1 30 9a46.883 46.883 0 0 1 24.064 6.5 6.931 6.931 0 0 0-3.499-3.84Z"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                          <path
                            d="M2 49.14V52a1 1 0 0 0 1 1h1.59a1.977 1.977 0 0 0 1.468-.64l.038-.041c.778-20.353 3.346-31.664 5.223-37.373a37.7 37.7 0 0 0-5.905 3.266L2.123 46.983A18.241 18.241 0 0 0 2 49.14ZM57 53a1 1 0 0 0 1-1v-2.86a18.064 18.064 0 0 0-.123-2.151l-3.291-28.778a37.851 37.851 0 0 0-5.905-3.265c1.877 5.709 4.445 17.019 5.223 37.372l.038.041A1.974 1.974 0 0 0 55.41 53Z"
                            opacity="1"
                            data-original="#000000"
                            class=""
                          ></path>
                        </g>
                      </svg>
                    </div>
                    <p class="hoodColor"></p>
                  </div>
                </div>
              </div>
              <div class="link"></div>
            </div>
          </div>
        </div>
      </main>
    </ion-content>
  </ion-page>
</template>

<style scoped>
.ion-page {
  height: 100vh;
  overflow: hidden;
}

.title {
  position: absolute;
  z-index: 1;
  left: 50%;
  transform: translate(-50%, -15%);
  margin-bottom: 3px;
}

.fil12 {
  fill: white;
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

.carInfo {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #0089c1;
  width: 100%;
  height: 35%;
  border-radius: 0px 0px 0px 50px;
  padding: 20px;
}

.carImg {
  width: 100%;
  padding: 0px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.carName {
  position: absolute;
  top: 31%;
  color: white;
  margin: 0;
  font-size: 1.5rem;
}

.menu-page {
  background-color: white;
  width: 100vw;
  height: 100vh;
}

.menu-page-inner {
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
  text-align: center;
  padding-top: 1.5rem;
  gap: 1rem;
}

.moreInfos {
  border-radius: 25px;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}

.moreInfos .moreInfos-inner {
  height: 30%;
  width: 85%;
  display: flex;
  flex-direction: column;
  justify-content: start;
  gap: 1rem;
}

.moreInfos .moreInfos-inner:nth-child(2) {
  height: 60%;
  width: 90%;
  display: flex;
  flex-direction: column;
  justify-content: start;
  background-color: #0089c1;
  border-radius: 20px;
  margin: 20px 0px;
  padding: 10px;
  gap: 0.7rem;
}

.block {
  display: flex;
  width: 100%;
  height: 100%;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 0.7rem;
}

.blocks {
  width: 100%;
  height: fit-content;
  display: flex;
  flex-direction: row;
  justify-content: start;
  align-items: center;
  gap: 0.7rem;
}

.blocks p {
  margin: 0px;
  height: 30%;
  color: #0089c1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.moreInfos .moreInfos-inner:nth-child(2) .blocks p {
  color: white;
}

.link {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  bottom: 0px;
}

.infoIcons {
  width: 3rem;
  height: 3rem;
  fill: white;
}

.roof {
  width: 2rem;
  height: 2rem;
  fill: white;
}

.moreInfos .moreInfos-inner:nth-child(2) .infoIcons {
  width: 3rem;
  height: 3rem;
  fill: #0089c1;
}

.moreInfos .moreInfos-inner:nth-child(2) .roof {
  width: 2rem;
  height: 2rem;
  fill: #0089c1;
}

.moreInfos .moreInfos-inner:nth-child(2) .icons-circle {
  background-color: white;
}

.icons-circle {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 3rem;
  height: 3rem;
  background-color: #0089c1;
  padding: 0.7rem;
  border-radius: 500px;
}

.menu-page p {
  font-size: 1.2rem;
  text-transform: capitalize;
  font-weight: 600;
  color: #0089c1;
  text-align: start;
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
import jsonData from "@/components/json/colorsName.json";
import { ref } from "vue";

export default {
  components: {
    IonPage,
    IonContent,
    IonButton,
    useRouter,
    useBackButton,
    useIonRouter,
    ref,
  },

  data() {
    return {
      data: jsonData,
    };
  },

  computed: {},

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
      let cName, cYear, cImage, ciUrl, wBrand, wType;

      cImage = document.querySelector(".carImg");
      cName = document.querySelector(".carName");
      wBrand = document.querySelector(".brand");
      wType = document.querySelector(".type");
      ciUrl = localStorage.getItem("carUrl");
      cYear = localStorage.getItem("carYear");

      //print car image
      cImage.innerHTML = `<img src="/assets/scenes/${ciUrl}.png" style="width:60%" >`;

      //Print car name and year
      cName.innerHTML =
        localStorage.getItem("carName") + " " + localStorage.getItem("carYear");

      //Print vinil brand
      wBrand.innerHTML = localStorage.getItem("brandWrapSel");

      //Print type of vinil
      wType.innerHTML = localStorage.getItem("wrapTypeSel");

      //Print colors name
      let data,
        indexD,
        cWrap,
        reWrap,
        roWrap,
        hoWrap,
        cBrand,
        send,
        boColor,
        roColor,
        reColor,
        hoColor;

      indexD = jsonData;
      data = indexD[0];

      boColor = localStorage.getItem("bColor");
      roColor = localStorage.getItem("roColor");
      reColor = localStorage.getItem("reColor");
      hoColor = localStorage.getItem("hoColor");

      //Collect the informations in labels to send
      send = document.querySelector(".link");
      cWrap = document.querySelector(".infoColor");
      reWrap = document.querySelector(".retroColor");
      roWrap = document.querySelector(".roofColor");
      hoWrap = document.querySelector(".hoodColor");
      cBrand =
        localStorage.getItem("brandWrapSel").substr(0, 1).toUpperCase() +
        localStorage.getItem("brandWrapSel").substr(1);

      function c1() {
        if (data[boColor] == undefined) {
          cWrap.innerHTML = "";
        } else {
          cWrap.innerHTML = data[boColor];
        }
      }

      function c2() {
        if (data[roColor] == undefined) {
          roWrap.innerHTML = "";
        } else {
          roWrap.innerHTML = data[roColor];
        }
      }

      function c3() {
        if (data[reColor] == undefined) {
          reWrap.innerHTML = "";
        } else {
          reWrap.innerHTML = data[reColor];
        }
      }

      function c4() {
        if (data[hoColor] == undefined) {
          hoWrap.innerHTML = "";
        } else {
          hoWrap.innerHTML = data[hoColor];
        }
      }

      //Write in labels
      c1();
      c2();
      c3();
      c4();

      //Compose presuposto button
      send.innerHTML = `<a href="https://wa.me/34698272509?text=Me+gustaría+una+cotización+para+mi ${localStorage.getItem(
        "carName"
      )} ${cYear}%0DVinilo elegido: ${cBrand}%0DTipo de vinilo: ${localStorage.getItem(
        "wrapTypeSel"
      )}%0DCoche entero: ${data[boColor]}%0DTecho: ${
        data[roColor]
      }%0DVista trasera: ${data[reColor]}%0DCapucha: ${
        data[hoColor]
      }" class="presuposto" style="display: block; border-radius: 15px 15px 0px 0px;background-color: #0089c1; font-size: 1.2rem;padding: 18px 0px; width: 100%; color: white; font-weight: 700; text-decoration: none;">Pedir presupuesto</a>`;
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
