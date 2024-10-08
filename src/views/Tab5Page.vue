<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div class="top-bar-showroom">
        <div class="menu-title">
          <a class="showroom-btn" v-on:click="clear"
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
                  fill="#49ade7"
                  opacity="1"
                  data-original="#49ade7"
                ></path>
              </g>
            </svg>
          </a>

          <div id="vinil-brand"></div>

          <ion-button class="showroom-menu" router-link="/tabs/tab7">
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
          </ion-button>
        </div>
      </div>
      <main>
        <div id="car"></div>
        <div class="carPart">
          <div class="btnR" style="display: none">
            <div class="btnR-inner">
              <button class="bodywork">
                <svg class="icons" viewBox="-1.5 0 32 32" fill="#000000">
                  <g stroke-width="0"></g>
                  <g stroke-linecap="round" stroke-linejoin="round"></g>
                  <g>
                    <g></g>
                    <path
                      d="M5.867 15.467c-1.173 0-2.133 0.96-2.133 2.133s0.96 2.133 2.133 2.133 2.133-0.96 2.133-2.133-0.96-2.133-2.133-2.133zM5.867 18.667c-0.587 0-1.067-0.48-1.067-1.067s0.48-1.067 1.067-1.067c0.587 0 1.067 0.48 1.067 1.067s-0.48 1.067-1.067 1.067z"
                      fill="#49ade7"
                    ></path>
                    <path
                      d="M22.933 15.467c-1.173 0-2.133 0.96-2.133 2.133s0.96 2.133 2.133 2.133c1.173 0 2.133-0.96 2.133-2.133s-0.96-2.133-2.133-2.133zM22.933 18.667c-0.587 0-1.067-0.48-1.067-1.067s0.48-1.067 1.067-1.067c0.587 0 1.067 0.48 1.067 1.067s-0.48 1.067-1.067 1.067z"
                      fill="#49ade7"
                    ></path>
                    <path
                      d="M25.12 11.2l-0.907-4.267c-0.373-1.387-1.44-2.133-2.88-2.133h-13.867c-1.493 0-2.347 0.747-2.773 2.133l-0.96 4.267h-3.733v1.067h3.467v0.053c-1.653 0.107-2.933 1.493-2.933 3.2v7.413h1.6v1.6c0 1.493 1.173 2.667 2.667 2.667s2.667-1.173 2.667-2.667v-1.6h13.867v1.6c0 1.493 1.173 2.667 2.667 2.667s2.667-1.173 2.667-2.667v-1.6h1.6v-7.413c0-1.653-1.28-3.040-2.88-3.2v-0.053h3.413v-1.067h-3.68zM5.707 7.253c0.32-0.96 0.8-1.387 1.76-1.387h13.867c1.013 0 1.6 0.427 1.867 1.333l1.067 5.12h-19.733l1.173-5.067zM6.4 24.533c0 0.907-0.693 1.6-1.6 1.6s-1.6-0.693-1.6-1.6v-1.6h3.2v1.6zM25.6 24.533c0 0.907-0.693 1.6-1.6 1.6s-1.6-0.693-1.6-1.6v-1.6h3.2v1.6zM27.2 15.52v6.347h-25.6v-6.347c0-1.173 0.96-2.133 2.133-2.133h21.333c1.173 0 2.133 0.96 2.133 2.133z"
                      fill="#49ade7"
                    ></path>
                  </g>
                </svg>
              </button>
              <button class="roof">
                <svg
                  class="icons"
                  xml:space="preserve"
                  style="
                    shape-rendering: geometricPrecision;
                    text-rendering: geometricPrecision;
                    image-rendering: optimizeQuality;
                    fill-rule: evenodd;
                    clip-rule: evenodd;
                  "
                  viewBox="0 0 65.54 107.67"
                >
                  <g>
                    <metadata />
                    <path
                      class="fil12"
                      d="M61.89 43.48c-1.59,0 -3.16,0.43 -4.6,-0.26 0.19,-2.37 3.64,-1.56 4.6,0.26zm-21.74 64.19l-13.3 0c-3.85,-0.15 -7.56,-0.61 -12.97,-1.86 -3.9,-0.9 -3.79,-1.55 -4.12,-3.05l-1.31 -10.71c-0.14,-2.73 -1.55,-1.61 -1.55,-3.05l0 -8.19c0,-1.89 0.89,-1.79 1.03,-3.58l-0.01 -8.95c-0.01,-1.75 0.28,-2.34 0.27,-4.08 -0.01,-1.54 0,-3.08 -0.01,-4.61 -0.01,-1.8 0.25,-2.56 0.27,-4.08 0.04,-3.22 0.25,-5.65 0.25,-8.71 -2.25,0.52 -5.08,0.4 -7.21,-0.47 -0.96,-0.39 -1.39,-1.09 -1.49,-1.89l0 -0.75c0.18,-1.7 1.47,-3.58 2.31,-4.05 1.38,-0.77 3.77,-1.02 5.87,-1.02l-1.07 -8.22c0.23,-4.19 0.12,-2.47 -0.69,-3.82 -0.65,-1.08 -0.42,-8.35 -0.2,-9.61 0.29,-1.63 0.78,-1.49 1.67,-2.44 0.95,-1.02 0.41,-1.71 0.65,-3.43 1.02,-7.24 0.21,-8.92 6.9,-9.98 4.34,-0.68 11.2,-1.12 15.5,-1.12 2.86,0 14.06,0.29 15.76,0.61 1.13,0.21 1.07,0.38 2.4,0.41 6.87,0.18 7.31,3.29 7.69,8.68l0.67 4.7c0.72,1.49 2.42,0.77 2.17,5.58 -0.04,0.88 -0.24,2.64 -0.23,3.05 0.03,1.27 0.6,0.86 0.09,2.42l-1.18 2.17c0,1.37 0.31,1.6 0.2,2.74 -0.06,0.56 -0.36,2.04 -0.42,2.67 -0.22,2.12 -0.12,3.74 -0.55,5.59 1.76,-0.41 1.59,-0.36 3.01,0.06 2.76,0.81 4.05,1.11 4.74,4.22 0.37,1.64 0.57,2.46 -1.1,3.39 -1.67,0.93 -5.11,0.99 -7.16,0.51 0,6.04 0.51,11.65 0.51,17.9 0,1.31 -0.48,0.47 -0.04,2.07 0.86,3.13 -0.09,7.94 0.29,11.23 0.16,1.35 0.27,0.57 0.71,1.6 0.54,1.24 0.32,6.39 0.32,8.12 0,2.21 -0.97,2.22 -1.51,3.35 -0.36,0.76 -0.84,10.9 -1.81,12.76 -0.81,1.54 -5.3,2.46 -6.98,2.74 -1.6,0.28 -2.57,0.46 -4.25,0.61 -1.49,0.13 -2.36,0.49 -4.12,0.49zm-36.31 -64.19c0.44,-1.93 4.36,-2.41 4.6,-0.26 -1.46,0.7 -2.94,0.26 -4.6,0.26zm24.29 -39.9l9.46 0c0,1.32 -0.23,2.03 0.02,2.45 0.24,0.41 -0.01,0.06 0.8,0.57 1.4,0.87 7.94,1.84 9.92,1.84 1.83,0 1.7,-0.7 3.07,-1.02 -0.02,-1.13 -0.25,-1.2 -0.25,-2.56 0.74,0.06 1.13,0.09 1.4,0.68l0.38 1.35c0.62,2.22 1.01,9.34 1.44,12.4l0.62 8.58c0.1,1.87 -0.79,10.44 -1.11,12.71 -0.37,2.72 -0.19,10.04 -0.18,13.13 0,1.68 0.27,2.47 0.26,4.34l0.26 13.56c0,2.98 0.29,10.04 -0.27,12.54 -0.3,1.35 0.33,2.27 -0.18,4.93l-0.78 9.17c-0.18,1.42 -0.28,2.57 -0.56,3.79 -1.26,0.1 -3.11,0.73 -4.34,1.03 -0.77,0.19 -1.29,0.19 -2.2,0.36 -7.07,1.33 -16.13,1.07 -23.35,0.36l-7.2 -1.23c-0.85,-0.22 -1.24,-0.5 -2.3,-0.52l-0.81 -7.63c-0.12,-0.82 -0.14,-1.5 -0.25,-2.56 -0.73,-6.79 -0.45,-19.54 -0.47,-27.15 -0.01,-2.1 0.27,-3.23 0.26,-5.11l0.25 -10.75c0.06,-0.97 0.27,-1.21 0.16,-2.18l-1.19 -12.39c-0.03,-4.6 -0.58,-6.26 0.04,-11.98 0.19,-1.72 0.45,-4.59 0.48,-6.44l1.16 -9.32c0.27,-1.23 0.54,-1.64 1.91,-1.67 -1.89,3.94 3.22,3.67 5.14,3.5l5.93 -1.12c2.04,-0.38 2.48,-1.43 2.48,-3.66zm13.04 0.26c1.76,0 3.39,-0.1 5.14,0.23 0.97,0.19 0.72,-0.25 1,0.79 -2.58,0 -3.68,-0.77 -6.14,-0.77l0 -0.25zm-23.01 1.27c0.23,-0.46 0.19,-0.32 0.25,-1.02l4.3 -0.17c0.07,0 0.2,-0.06 0.58,-0.02l0.75 0.19c-1.76,0.15 -4.26,0.65 -5.88,1.02zm6.14 -1.53l0.07 0.08c0,-0.01 -0.1,-0.05 -0.07,-0.08z"
                    />
                    <path
                      class="fil12"
                      d="M46.03 97.44c-1.21,0.02 -2.02,0.4 -3.33,0.5 -1.4,0.12 -1.96,0.28 -3.57,0.27 -2.86,-0.04 -7.37,0.42 -10.49,0.25l-8.95 -1.02c0,-1.11 0.2,-1.95 0.26,-3.32l0.83 -6.33c0.12,-0.8 0.49,-1.99 0.7,-2.88 2.69,0 4.4,0.51 7.16,0.51l13.01 -0.3c0.9,-0.1 1.31,-0.21 2.59,-0.21 -0.19,2.35 0.79,2.75 1.01,5.9l0.78 6.63zm-18.41 4.34c6.7,0 13.56,0.43 20.01,-1.21 2.12,-0.53 1.73,-1.25 1.73,-4.41 0,-1.79 -0.48,-2.41 -0.52,-4.09 -0.03,-1.8 -0.87,-6.03 -1.32,-7.89 -0.47,-1.97 -0.53,-1.69 -1.49,-3.11 -1.62,0.04 -4.3,0.77 -7.67,0.77 -3.82,0 -12.63,0.36 -15.94,-0.41l-3.24 -0.36c-0.16,0.58 -0.55,0.94 -1.2,3.15 -0.35,1.23 -0.39,2.38 -0.66,3.69 -0.24,1.21 -1.69,10.63 -0.93,11.81 0.51,0.79 1.95,0.89 3.15,1.2 1.94,0.5 5.77,0.86 8.08,0.86z"
                    />
                    <path
                      class="fil12"
                      d="M43.22 45.52c-4.33,-1.01 -11.73,-1.72 -16.23,-0.88 -0.96,0.18 -1.54,0.37 -2.5,0.49l-2.24 0.39 -2.33 -6.62c-0.43,-1.48 -0.74,-1.89 -0.74,-3.86 2.77,-0.65 4.46,-1.55 8.71,-2.03 4.22,-0.48 11.12,-0.42 14.9,0.94 2.39,0.86 1.39,0.09 3.75,1.34 -0.1,1.28 -0.05,0.28 -0.32,1.22 -0.98,3.44 -1.04,4.92 -3,9.01zm-27.88 -11c0,1.11 1.81,6.91 2.16,8.08 2.79,9.34 4.79,6.09 9.16,5.54 4.63,-0.58 8.46,-0.4 12.97,0.21 4.44,0.6 6.28,3.77 9.73,-9.99 0.44,-1.77 0.53,-3.33 1.02,-4.35l-1.35 -1.45c-1.23,-0.74 -3.63,-1.58 -5.04,-1.87 -6.7,-1.38 -9,-2.02 -16.59,-1.25 -2.14,0.22 -6.85,1.41 -8.98,2.27 -1.28,0.52 -3.08,1.09 -3.08,2.81z"
                    />
                    <path
                      class="fil12"
                      d="M49.87 69.56c0.3,0.48 0.29,-0.57 0.21,0.51 -0.04,0.55 -0.03,0.23 -0.21,0.51l0 -1.02zm-0.26 -9.72l0.26 0 0 8.95 -0.26 0 0 -8.95zm-3.58 4.09c0,3.4 0.27,7.52 1.46,10.31 1.51,3.54 0.85,2.24 2.63,5.04 0.88,1.38 0.55,1.28 2.31,1.28 2.19,0 1.01,-7.27 1.02,-9.21 0.04,-7.14 -0.72,-16.9 -0.52,-23.54 0.03,-1.1 0.24,-1.44 0.28,-2.54 0.06,-1.56 0.02,-2.42 -0.86,-3.25 -2.04,-1.92 -3.05,1.69 -3.89,3.37 -0.9,1.8 -1.85,3.02 -1.92,5.24 -0.04,1.15 -0.38,2.27 -0.37,3.07 0,0.65 0.13,2.24 0.13,3.34 -0.01,1.53 -0.26,1.86 -0.28,3.3 -0.01,1.19 0.01,2.4 0.01,3.59z"
                    />
                    <path
                      class="fil12"
                      d="M15.6 69.05l0.08 0.08c-0.01,-0.01 -0.11,-0.06 -0.08,-0.08zm0.26 -9.72l0.25 0 0 8.7 -0.25 0 0 -8.7zm-3.07 -7.67c0,1.34 -0.36,2.2 -0.35,3.02 0.02,1.01 0.09,2.25 0.09,3.37 0,2.75 -0.26,4.49 -0.25,7.16 0,5.15 -0.26,9.42 -0.26,14.58 0.81,0.54 2.31,1.92 3.76,-0.84 1.7,-3.25 3.14,-6.33 3.71,-10.08 0.13,-0.9 -0.06,-0.37 -0.05,-1.6 0.02,-1.15 0.25,-2.26 0.25,-3.85 0.01,-2.53 -0.16,-12.42 -1.05,-14.8 -0.43,-1.18 -0.75,-1.68 -1.2,-2.63 -0.28,-0.58 -0.33,-0.82 -0.65,-1.41 -0.6,-1.13 -1.06,-3.06 -2.7,-3.01 -1.13,0.03 -1.52,1.26 -1.57,2.41l0.27 7.68z"
                    />
                  </g>
                </svg>
              </button>
              <button class="rearview">
                <svg
                  x="0"
                  y="0"
                  viewBox="0 0 512 512"
                  style="enable-background: new 0 0 512 512"
                  xml:space="preserve"
                  class="icons"
                >
                  <g>
                    <path
                      d="m402.917 236.302-26.209-78.583a74.585 74.585 0 0 0-70.833-51.052H185.438c-58.708 0-110.75 35.229-132.542 89.74-6.792 16.938-10.229 34.781-10.229 53.031 0 27.146 22.083 49.229 49.229 49.229h266.063c26.125 0 47.375-21.25 47.375-47.375 0-5.042-.813-10.063-2.417-14.99zm-44.959 41.031H91.896c-15.375 0-27.896-12.51-27.896-27.896 0-15.521 2.917-30.698 8.688-45.104C91.25 157.969 135.5 128 185.438 128h120.438c23 0 43.313 14.656 50.583 36.469L382.646 243a26.473 26.473 0 0 1 1.354 8.292c0 14.354-11.687 26.041-26.042 26.041z"
                      fill="#49ade7"
                      opacity="1"
                      data-original="#000000"
                      class=""
                    ></path>
                    <path
                      d="M501.333 149.333H480c-5.604 0-10.25 4.323-10.646 9.906-.038.499-3.667 45.814-29.471 53.03l-22.695-68.04A117.187 117.187 0 0 0 305.875 64H185.438c-76.25 0-143.833 45.75-172.146 116.542C4.479 202.542 0 225.719 0 249.438c0 50.667 41.229 91.896 91.896 91.896H352c67.146 0 117.958 99.771 118.458 100.771a10.671 10.671 0 0 0 9.542 5.896h21.333A10.66 10.66 0 0 0 512 437.334V160a10.66 10.66 0 0 0-10.667-10.667zM91.896 319.998V320c-38.917 0-70.563-31.656-70.563-70.563 0-20.99 3.958-41.5 11.75-60.969 25.063-62.656 84.875-103.135 152.354-103.135h120.438a95.877 95.877 0 0 1 91.063 65.646l26.188 78.51c2.354 7.188 3.542 14.521 3.542 21.802 0 37.885-30.813 68.708-68.708 68.708H91.896zm398.771 106.669h-4.25c-9.926-17.978-42.359-71.186-88.84-94.923C427.316 317.024 448 286.657 448 251.292c0-6.15-.879-12.296-2.156-18.418 30.441-8.217 40.438-44.357 43.51-62.207h1.313v256z"
                      fill="#49ade7"
                      opacity="1"
                      data-original="#000000"
                      class=""
                    ></path>
                    <path
                      d="M188.876 173.792c-4.168-4.167-10.918-4.167-15.084 0l-64 64c-4.167 4.167-4.167 10.917 0 15.083a10.634 10.634 0 0 0 7.542 3.125c2.729 0 5.458-1.042 7.542-3.125l64-64c4.167-4.167 4.167-10.917 0-15.083zM135.541 173.792c-4.167-4.167-10.917-4.167-15.083 0l-21.333 21.333c-4.167 4.167-4.167 10.917 0 15.083 2.083 2.083 4.813 3.125 7.542 3.125s5.458-1.041 7.541-3.125l21.333-21.333c4.167-4.167 4.167-10.917 0-15.083z"
                      fill="#49ade7"
                      opacity="1"
                      data-original="#000000"
                      class=""
                    ></path>
                  </g>
                </svg>
              </button>
              <button class="hood">
                <svg
                  x="0"
                  y="0"
                  viewBox="0 0 60 60"
                  style="enable-background: new 0 0 512 512"
                  xml:space="preserve"
                  class="icons"
                >
                  <g
                    transform="matrix(-1,-1.2246467991473532e-16,1.2246467991473532e-16,-1,59.99999686206865,59.99898719787599)"
                  >
                    <path
                      d="M56.453 16.947a8.939 8.939 0 0 0-5.021-7.09 49.711 49.711 0 0 0-42.867 0 8.936 8.936 0 0 0-5.018 7.087l-3.41 29.8A20.156 20.156 0 0 0 0 49.14V52a3 3 0 0 0 3 3h1.59a3.975 3.975 0 0 0 2.951-1.3C9.907 51.085 16.832 45 30 45s20.093 6.085 22.458 8.7A3.976 3.976 0 0 0 55.41 55H57a3 3 0 0 0 3-3v-2.86a19.979 19.979 0 0 0-.137-2.383ZM9.432 11.662a47.7 47.7 0 0 1 41.133 0 6.931 6.931 0 0 1 3.5 3.838A46.883 46.883 0 0 0 30 9a46.868 46.868 0 0 0-24.064 6.5 6.924 6.924 0 0 1 3.496-3.838ZM28 11.052c.658-.028 1.319-.052 2-.052s1.342.024 2 .052V38a1 1 0 0 1-1 1h-2a1 1 0 0 1-1-1ZM4.59 53H3a1 1 0 0 1-1-1v-2.86a18.241 18.241 0 0 1 .123-2.157l3.291-28.771a37.7 37.7 0 0 1 5.905-3.266C9.442 20.655 6.874 31.966 6.1 52.319l-.038.041A1.977 1.977 0 0 1 4.59 53Zm3.592-2.687C9.177 28.622 12.307 17.9 13.8 13.926A45.632 45.632 0 0 1 26 11.183V38a3 3 0 0 0 3 3h2a3 3 0 0 0 3-3V11.183a45.632 45.632 0 0 1 12.2 2.743c1.491 3.975 4.621 14.695 5.616 36.386C48.17 47.2 41.188 43 30 43s-18.17 4.2-21.818 7.313ZM58 52a1 1 0 0 1-1 1h-1.59a1.974 1.974 0 0 1-1.468-.641l-.038-.041c-.778-20.353-3.346-31.663-5.223-37.372a37.851 37.851 0 0 1 5.905 3.265l3.291 28.778A18.064 18.064 0 0 1 58 49.14Z"
                      fill="#49ade7"
                      opacity="1"
                      data-original="#000000"
                      class=""
                    ></path>
                  </g>
                </svg>
              </button>
              <div class="hidenCircle"></div>
            </div>
          </div>
          <button id="reveal" class="button">
            <div id="wrapper" class="wrapper">
              <span class="tag-wrapper">
                <span id="tag" class="icon tag">
                  <svg
                    x="0"
                    y="0"
                    viewBox="0 0 512 512"
                    style="enable-background: new 0 0 512 512"
                    xml:space="preserve"
                    class="arrowUpR"
                  >
                    <g>
                      <path
                        d="M501.818 90.998a15.118 15.118 0 0 0-24.749-5.118l-77.994 77.994-41.932-9.016-9.015-41.932 77.994-77.995a15.125 15.125 0 0 0-5.118-24.75C367.457-11.053 306.542 1.538 265.818 42.26c-19.604 19.604-33.066 44.227-38.93 71.206a144.544 144.544 0 0 0 1.991 69.544L20.735 391.154C7.363 404.524 0 422.301 0 441.21s7.363 36.686 20.734 50.056C34.105 504.637 51.881 512 70.79 512c18.908 0 36.686-7.363 50.056-20.734L328.99 283.122a144.565 144.565 0 0 0 69.543 1.99c26.98-5.864 51.603-19.326 71.207-38.93 40.723-40.722 53.313-101.637 32.078-155.184z"
                        fill="#49ade7"
                        opacity="1"
                        data-original="#000000"
                        class=""
                      ></path>
                    </g>
                  </svg>
                </span>
              </span>
              <span id="close" class="close"></span>
            </div>
          </button>
        </div>

        <ion-button router-link="/tabs/tab6" class="sendBt">
          <svg
            x="0"
            y="0"
            viewBox="0 0 24 24"
            style="enable-background: new 0 0 512 512"
            xml:space="preserve"
            class="icon"
          >
            <g
              transform="matrix(1.2100000000000002,0,0,1.2100000000000002,-2.5200000500679014,-2.480294952392578)"
            >
              <path
                d="M9.707 19.121a.997.997 0 0 1-1.414 0l-5.646-5.647a1.5 1.5 0 0 1 0-2.121l.707-.707a1.5 1.5 0 0 1 2.121 0L9 14.171l9.525-9.525a1.5 1.5 0 0 1 2.121 0l.707.707a1.5 1.5 0 0 1 0 2.121z"
                fill="#49ade7"
                opacity="1"
                data-original="#000000"
                class=""
              ></path>
            </g>
          </svg>
        </ion-button>

        <div class="colors-container">
          <div class="main-colors">
            <div class="colors"></div>
            <button id="upBtn">
              <svg
                fill="#49ade7"
                class="arrowUp"
                version="1.1"
                id="Layer_1"
                viewBox="0 0 330 330"
                xml:space="preserve"
              >
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g
                  id="SVGRepo_tracerCarrier"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></g>
                <g id="SVGRepo_iconCarrier">
                  <path
                    id="XMLID_224_"
                    d="M325.606,229.393l-150.004-150C172.79,76.58,168.974,75,164.996,75c-3.979,0-7.794,1.581-10.607,4.394 l-149.996,150c-5.858,5.858-5.858,15.355,0,21.213c5.857,5.857,15.355,5.858,21.213,0l139.39-139.393l139.397,139.393 C307.322,253.536,311.161,255,315,255c3.839,0,7.678-1.464,10.607-4.394C331.464,244.748,331.464,235.251,325.606,229.393z"
                  ></path>
                </g>
              </svg>
            </button>
          </div>
          <div class="other-colors">
            <div class="colors2"></div>
          </div>
        </div>
      </main>
    </ion-content>
  </ion-page>
</template>

<style scoped>
.fil12 {
  fill: #49ade7;
}

main {
  background: black;
  background-position: center center;
  background-size: cover;
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
}

.top-bar-showroom {
  height: 4.4rem;
  width: 100%;
  border-radius: 0px 0px 30px 30px;
  position: fixed;
  top: 0;
  z-index: 99;
}

.showroom-btn {
  background-color: white;
  width: 2.7rem;
  height: 2.7rem;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 500px;
  padding-right: 4px;
}

.showroom-menu {
  background-color: white;
  width: 2.7rem;
  height: 2.7rem;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 500px;
  --box-shadow: none;
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

.menu-svg {
  height: 1.3rem;
}

#vinil-brand {
  background-color: white;
  width: 50%;
  height: 2.7rem;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
}

.car {
  width: 100%;
  height: calc(100% - 11.4rem);
  background-color: transparent;
}

.carPart {
  position: fixed;
  left: 1rem;
  bottom: 9rem;
  z-index: 98;
  display: flex;
  flex-direction: column;
}

#reveal {
  background-color: white;
  width: 3.5rem;
  height: 3.5rem;
  border-radius: 500px;
  padding: 0.7rem;
  position: fixed;
  left: 1rem;
  bottom: 8rem;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0px 15px 35px -5px rgb(50 88 130 / 32%);
  transform: scale(1) translateY(0);
  transition: transform 250ms ease;
  &:focus {
    animation: button-click 300ms ease 0ms 1;
  }
  &:active {
    animation: none;
  }
}

.sendBt {
  background-color: white;
  width: 3.5rem;
  height: 3.5rem;
  border-radius: 500px;
  padding: 0.7rem;
  position: fixed;
  right: 1rem;
  bottom: 8rem;
  --box-shadow: none;
}

.sendBt .icon {
  height: 1.6rem;
  width: 1.6rem;
}

.btnR {
  display: none;
  flex-direction: column;
  gap: 1rem;
  border-radius: 500px;
}

.btnR-inner {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  border-radius: 500px;
}

.arrowUpR {
  height: 1.5rem;
  width: 1.5rem;
  rotate: 0deg;
}

.carPart button {
  background-color: white;
  width: 3.5rem;
  height: 3.5rem;
  border-radius: 500px;
  padding: 0.7rem;
}

.active-btn {
  background-color: #f3f3f3 !important;
  border: 3px solid #49ade7;
}

.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.tag-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  transform: scale(1);
}

.tag {
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #49ade7;
  transform: rotate(-90deg);
  cursor: pointer;
}

.close {
  display: none;
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  background: none;
  width: 75px;
  height: 75px;
  transform-origin: center;
  &::before,
  &::after {
    content: "";
    position: absolute;
    background: #49ade7;
    width: 4px;
    height: 1.5rem;
    top: 1.6rem;
    border-radius: 4px;
    opacity: 0;
    transform: scale(1);
  }
}

.wrapper.open .tag-wrapper {
  transform: scaleX(0);
}

.wrapper.open .close {
  display: flex;
  &::before,
  &::after {
    display: flex;
    top: 1.6rem;
    opacity: 1;
  }
  &::before {
    transform: scale(0.9) rotate(-45deg);
  }
  &::after {
    transform: scale(0.9) rotate(45deg);
  }
}

.carPart .hidenCircle {
  background-color: transparent;
  width: 2.5rem;
  height: 2.5rem;
  border-radius: 500px;
  padding: 0.7rem;
}

.icons {
  width: 100%;
  height: 100%;
}
.colors-container {
  width: 100%;
  background-color: white;
  height: fit-content;
  border-radius: 30px 30px 0px 0px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: fixed;
  bottom: 0;
  z-index: 98;
  padding: 0px 1rem;
}

.main-colors {
  height: 7rem;
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.colors {
  width: 80%;
  height: 3rem;
  background-color: #ecebeb;
  border-radius: 10px;
  padding: 0px 1rem;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

#upBtn {
  width: 2rem;
  height: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  background: transparent;
}

.arrowUp {
  height: 1.5rem;
  width: 1.5rem;
  rotate: 0deg;
}

.rotate {
  rotate: 180deg;
}

.other-colors {
  width: 95%;
  height: 20rem;
  background-color: #ecebeb;
  border-radius: 10px;
  padding: 1rem;
  margin-bottom: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.colors2 {
  width: 100%;
  height: 100%;
  background-color: #ecebeb;
  border-radius: 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
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
import * as THREE from "three";
import { OrbitControls } from "three/addons/controls/OrbitControls.js";
import { GLTFLoader } from "three/examples/jsm/loaders/GLTFLoader";
import { DRACOLoader } from "three/examples/jsm/loaders/DRACOLoader";
import { useRouter } from "vue-router";

export default {
  components: {
    IonPage,
    IonContent,
    THREE,
    OrbitControls,
    GLTFLoader,
    DRACOLoader,
    IonButton,
    useRouter,
    useBackButton,
    useIonRouter,
  },

  setup() {
    let camera,
      scene,
      renderer,
      car,
      canvas,
      ren,
      backBt,
      shadow,
      model,
      alias,
      shadowRaw,
      aliasRaw;

    setTimeout(() => {
      let wlg, lg, othersColors;

      //show wrap brand logo
      wlg = localStorage.getItem("brandWrapSel");
      lg = document.querySelector("#vinil-brand");

      if (wlg == "3m" || wlg == "imageP") {
        lg.innerHTML = `<img src="assets/img/wrapBrandLogos/${wlg}.png" style="width:70%" >`;
      } else {
        lg.innerHTML = `<img src="assets/img/wrapBrandLogos/${wlg}.png" style="width:55%" >`;
      }

      othersColors = document.querySelector(".other-colors");
      othersColors.style.display = "none";

      let vinils, vinil, mainColors, hideColors;

      vinils = localStorage.getItem("colorGroup");
      vinil = vinils.split(",");

      mainColors = document.querySelector(".colors");
      hideColors = document.querySelector(".colors2");

      //Colors
      for (let i = 0; i < vinils.length; i++) {
        if (i <= 4) {
          mainColors.innerHTML += `<button class="itemBo" value=${vinil[i]} style="width:2.3rem; height:2.3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
        } else if (i > 4 && i < 25) {
          hideColors.innerHTML += `<button class="itemBo" value=${vinil[i]} style="width:3rem; height:3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
        }
      }

      //Lift colors page
      let upBt, arrow;

      upBt = document.querySelector("#upBtn");
      arrow = document.querySelector(".arrowUp");

      upBt.addEventListener("click", () => {
        arrow.classList.toggle("rotate");
        if (othersColors.style.display === "none") {
          othersColors.style.display = "block";
        } else {
          othersColors.style.display = "none";
        }
      });

      //Reveal hide buttons
      let wrench, hideBts;

      wrench = document.querySelector("#wrapper");
      hideBts = document.querySelector(".btnR");

      wrench.addEventListener("click", function () {
        this.classList.toggle("open");
        if (hideBts.style.display === "none") {
          hideBts.style.display = "block";
        } else {
          hideBts.style.display = "none";
        }
      });

      //Active class in buttons
      let bodywork, rearview, roof, hood;

      bodywork = document.querySelector(".bodywork");
      rearview = document.querySelector(".rearview");
      roof = document.querySelector(".roof");
      hood = document.querySelector(".hood");

      bodywork.addEventListener("click", function (e) {
        let itemBo, itemRe, itemRo, itemHo;

        roof.classList.remove("active-btn");
        rearview.classList.remove("active-btn");
        hood.classList.remove("active-btn");
        bodywork.classList.add("active-btn");
        itemBo = document.querySelectorAll(".itemBo");
        itemRe = document.querySelectorAll(".itemRe");
        itemRo = document.querySelectorAll(".itemRo");
        itemHo = document.querySelectorAll(".itemHo");

        itemRe.forEach((c) => c.remove());
        itemRo.forEach((c) => c.remove());
        itemBo.forEach((c) => c.remove());
        itemHo.forEach((c) => c.remove());
        for (let i = 0; i < vinils.length; i++) {
          if (i <= 4) {
            mainColors.innerHTML += `<button class="itemBo" value=${vinil[i]} style="width:2.3rem; height:2.3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          } else if (i > 4 && i < 25) {
            hideColors.innerHTML += `<button class="itemBo" value=${vinil[i]} style="width:3rem; height:3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          }
        }
      });

      roof.addEventListener("click", function (e) {
        let itemBo, itemRe, itemRo, itemHo;

        bodywork.classList.remove("active-btn");
        rearview.classList.remove("active-btn");
        hood.classList.remove("active-btn");
        roof.classList.add("active-btn");
        itemBo = document.querySelectorAll(".itemBo");
        itemRe = document.querySelectorAll(".itemRe");
        itemRo = document.querySelectorAll(".itemRo");
        itemHo = document.querySelectorAll(".itemHo");

        itemRe.forEach((c) => c.remove());
        itemRo.forEach((c) => c.remove());
        itemBo.forEach((c) => c.remove());
        itemHo.forEach((c) => c.remove());
        for (let i = 0; i < vinils.length; i++) {
          if (i <= 4) {
            mainColors.innerHTML += `<button class="itemRo" value=${vinil[i]} style="width:2.3rem; height:2.3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          } else if (i > 4 && i < 25) {
            hideColors.innerHTML += `<button class="itemRo" value=${vinil[i]} style="width:3rem; height:3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          }
        }
      });

      rearview.addEventListener("click", function (e) {
        let itemBo, itemRe, itemRo, itemHo;

        bodywork.classList.remove("active-btn");
        roof.classList.remove("active-btn");
        hood.classList.remove("active-btn");
        rearview.classList.add("active-btn");
        itemBo = document.querySelectorAll(".itemBo");
        itemRe = document.querySelectorAll(".itemRe");
        itemRo = document.querySelectorAll(".itemRo");
        itemHo = document.querySelectorAll(".itemHo");

        itemRe.forEach((c) => c.remove());
        itemRo.forEach((c) => c.remove());
        itemBo.forEach((c) => c.remove());
        itemHo.forEach((c) => c.remove());
        for (let i = 0; i < vinils.length; i++) {
          if (i <= 4) {
            mainColors.innerHTML += `<button class="itemRe" value=${vinil[i]} style="width:2.3rem; height:2.3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          } else if (i > 4 && i < 25) {
            hideColors.innerHTML += `<button class="itemRe" value=${vinil[i]} style="width:3rem; height:3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          }
        }
      });

      hood.addEventListener("click", function (e) {
        let itemBo, itemRe, itemRo, itemHo;

        bodywork.classList.remove("active-btn");
        roof.classList.remove("active-btn");
        rearview.classList.remove("active-btn");
        hood.classList.add("active-btn");
        itemBo = document.querySelectorAll(".itemBo");
        itemRe = document.querySelectorAll(".itemRe");
        itemRo = document.querySelectorAll(".itemRo");
        itemHo = document.querySelectorAll(".itemHo");

        itemRe.forEach((c) => c.remove());
        itemRo.forEach((c) => c.remove());
        itemBo.forEach((c) => c.remove());
        itemHo.forEach((c) => c.remove());
        for (let i = 0; i < vinils.length; i++) {
          if (i <= 4) {
            mainColors.innerHTML += `<button class="itemHo" value=${vinil[i]} style="width:2.3rem; height:2.3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          } else if (i > 4 && i < 25) {
            hideColors.innerHTML += `<button class="itemHo" value=${vinil[i]} style="width:3rem; height:3rem; border-radius: 10px; background: #${vinil[i]}" ></button>`;
          }
        }
      });
    }, 5);

    //Render
    setTimeout(() => {
      shadowRaw = localStorage.getItem("shadow");
      shadow = shadowRaw === "true";
      aliasRaw = localStorage.getItem("alias");
      alias = aliasRaw === "true";
      model = localStorage.getItem("model");

      camera = new THREE.PerspectiveCamera(
        55,
        window.innerWidth / window.innerHeight,
        0.1,
        15
      );

      camera.aspect = window.innerWidth / window.innerHeight;
      camera.updateProjectionMatrix();
      camera.position.set(5, 0, 8);
      camera.lookAt(0, 0, 0);

      scene = new THREE.Scene();

      // Lights

      let spotLight = new THREE.SpotLight(0xffffff, 250);
      spotLight.position.set(0, 10, 0);
      spotLight.distance = 20;
      spotLight.angle = 0.4;
      spotLight.penumbra = 0.5;
      spotLight.castShadow = shadow;
      spotLight.shadow.mapSize.width = 1024;
      spotLight.shadow.mapSize.height = 1024;
      scene.add(spotLight);

      let dirlight = new THREE.DirectionalLight(0xffffff, 2);
      dirlight.position.set(5, 0, 0);
      dirlight.castShadow = shadow;
      scene.add(dirlight);

      let dirlight2 = new THREE.DirectionalLight(0xffffff, 2);
      dirlight2.position.set(-5, 0, 0);
      dirlight2.castShadow = shadow;
      scene.add(dirlight2);

      let dirlight3 = new THREE.DirectionalLight(0xffffff, 2);
      dirlight3.position.set(0, 0, 5);
      dirlight3.castShadow = shadow;
      scene.add(dirlight3);

      let dirlight4 = new THREE.DirectionalLight(0xffffff, 2);
      dirlight4.position.set(0, 0, -5);
      dirlight4.castShadow = shadow;
      scene.add(dirlight4);

      //Ground
      const ground = new THREE.Mesh(
        new THREE.PlaneGeometry(50, 50),
        new THREE.MeshPhongMaterial({ color: 0x555555 })
      );

      ground.rotation.x = -Math.PI / 2;
      ground.receiveShadow = true;
      scene.add(ground);

      //Model
      let loader = new GLTFLoader();
      let dloader = new DRACOLoader();
      dloader.setDecoderPath("assets/draco/javascript/");
      dloader.setDecoderConfig({ type: "js" });
      loader.setDRACOLoader(dloader);
      loader.load(
        `${localStorage.getItem("model")}${localStorage.getItem("carUrl")}.glb`,
        async (gltf) => {
          const model = gltf.scene;

          model.castShadow = shadow;
          model.traverse((child) => {
            child.castShadow = shadow;

            let bodyworkBt, rearviewBt, roofBt, hoodBt;

            bodyworkBt = document.querySelector(".bodywork");
            rearviewBt = document.querySelector(".rearview");
            roofBt = document.querySelector(".roof");
            hoodBt = document.querySelector(".hood");

            roofBt.classList.remove("active-btn");
            rearviewBt.classList.remove("active-btn");
            hoodBt.classList.remove("active-btn");
            bodyworkBt.classList.add("active-btn");

            let body, roof, rear, hood;

            body = child.getObjectByName("body");
            roof = child.getObjectByName("roof");
            rear = child.getObjectByName("rear");
            hood = child.getObjectByName("hood");

            //Colors when start canvas
            body?.traverse((wrap) => {
              if (wrap instanceof THREE.Mesh) {
                wrap.material.color.setHex(0xffffff);
                let cItem = document.querySelectorAll(".itemBo");
                cItem.forEach((ct) => {
                  ct.addEventListener("click", function (e) {
                    cItem.forEach((ci) => (ci.style.border = "0px"));

                    this.style.border = "3px solid #49ade7";

                    wrap.material.color.setHex(
                      "0x" + this.getAttribute("value")
                    );

                    localStorage.setItem("bColor", this.getAttribute("value"));
                  });
                });
              }
            });

            roof?.traverse((wrap) => {
              if (wrap instanceof THREE.Mesh) {
                wrap.material.color.setHex(0xffffff);
                let cItem = document.querySelectorAll(".itemBo");
                cItem.forEach((ct) => {
                  ct.addEventListener("click", function (e) {
                    cItem.forEach((ci) => (ci.style.border = "0px"));

                    this.style.border = "3px solid #49ade7";

                    wrap.material.color.setHex(
                      "0x" + this.getAttribute("value")
                    );

                    localStorage.setItem("roColor", this.getAttribute("value"));
                  });
                });
              }
            });

            rear?.traverse((wrap) => {
              if (wrap instanceof THREE.Mesh) {
                wrap.material.color.setHex(0xffffff);
                let cItem = document.querySelectorAll(".itemBo");
                cItem.forEach((ct) => {
                  ct.addEventListener("click", function (e) {
                    cItem.forEach((ci) => (ci.style.border = "0px"));

                    this.style.border = "3px solid #49ade7";

                    wrap.material.color.setHex(
                      "0x" + this.getAttribute("value")
                    );

                    localStorage.setItem("reColor", this.getAttribute("value"));
                  });
                });
              }
            });

            hood?.traverse((wrap) => {
              if (wrap instanceof THREE.Mesh) {
                wrap.material.color.setHex(0xffffff);
                let cItem = document.querySelectorAll(".itemBo");
                cItem.forEach((ct) => {
                  ct.addEventListener("click", function (e) {
                    cItem.forEach((ci) => (ci.style.border = "0px"));

                    this.style.border = "3px solid #49ade7";

                    wrap.material.color.setHex(
                      "0x" + this.getAttribute("value")
                    );

                    localStorage.setItem("hoColor", this.getAttribute("value"));
                  });
                });
              }
            });

            //Bodywork Button
            bodyworkBt.addEventListener("click", function (e) {
              setTimeout(() => {
                body?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemBo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "bColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });

                roof?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemBo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "roColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });

                rear?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemBo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "reColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });

                hood?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemBo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "reColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });
              }, 15);
            });

            //Roof Button
            roofBt.addEventListener("click", function (e) {
              setTimeout(() => {
                roof?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemRo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "roColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });
              }, 15);
            });

            //RearView Button
            rearviewBt.addEventListener("click", function (e) {
              setTimeout(() => {
                rear?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemRe");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "reColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });
              }, 15);
            });

            //CarHood Button
            hoodBt.addEventListener("click", function (e) {
              setTimeout(() => {
                hood?.traverse((wrap) => {
                  if (wrap instanceof THREE.Mesh) {
                    let cItem = document.querySelectorAll(".itemHo");
                    cItem.forEach((ct) => {
                      ct.addEventListener("click", function (e) {
                        cItem.forEach((ci) => (ci.style.border = "0px"));

                        this.style.border = "3px solid #49ade7";

                        wrap.material.color.setHex(
                          "0x" + this.getAttribute("value")
                        );

                        localStorage.setItem(
                          "hoColor",
                          this.getAttribute("value")
                        );
                      });
                    });
                  }
                });
              }, 15);
            });
          });

          await renderer.compileAsync(model, camera, scene);

          scene.add(model);
          render();
        }
      );

      // Renderer

      renderer = new THREE.WebGLRenderer({ antialias: alias });
      renderer.setSize(720, 1280);
      renderer.shadowMap.enabled = shadow;
      renderer.toneMapping = THREE.ACESFilmicToneMapping;
      renderer.toneMappingExposure = 1;

      car = document.querySelector("#car");
      car.appendChild(renderer.domElement);

      canvas = document.querySelector("canvas");
      canvas.style.width = "100vw";
      canvas.style.height = "100vh";

      // Controls

      let controls = new OrbitControls(camera, renderer.domElement);
      controls.target.set(0, 0.3, 0);
      controls.maxPolarAngle = 1.4;
      controls.enableDamping = false;
      controls.enablePan = false;
      controls.autoRotate = false;
      controls.minDistance = 6;
      controls.maxDistance = 12;
      controls.update();

      function render() {
        ren = requestAnimationFrame(render);
        renderer.render(scene, camera);
      }

      backBt = document.querySelector(".showroom-btn");

      backBt.addEventListener("click", function () {
        cancelAnimationFrame(ren);
        scene = null;
      });
    }, 10);

    let isCurrentView;

    useBackButton(9999, (processNextHandler) => {
      if (isCurrentView) {
        history.go(-1);
        cancelAnimationFrame(ren);
        scene = null;
      }
      processNextHandler();
    });
  },

  ionViewDidEnter() {
    this.isCurrentView = true;
  },

  ionViewDidLeave() {
    this.isCurrentView = false;
  },

  methods: {
    clear: function () {
      history.back();
    },
  },
};
</script>
