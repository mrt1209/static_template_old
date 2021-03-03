<template>
  <b-container fluid class="p-0" style="overflow-x: hidden">
    <div>
      <b-navbar class="d-flex" toggleable>
        <div id="center-nav" class="d-flex mx-auto">
          <!-- <div class="mx-auto" href="#"> -->
          <b-img
            id="shandon-logo"
            src="~/assets/Shandon_logo.png"
            fluid
            class="justify-content-center mx-auto my-auto"
          ></b-img>
          <b-navbar-toggle class="border-0" target="navbar-toggle-collapse">
            <!-- <template #default="{ expanded }">
            <p class="h1 mb-2">
              <b-icon v-if="expanded" icon="plus" variant="light"></b-icon>
              <b-icon v-else icon="plus" variant="light"></b-icon>
            </p>
          </template> -->
            <p class="h1 mb-2">
              <b-icon icon="plus" variant="light"></b-icon>
            </p>
          </b-navbar-toggle>

          <b-collapse id="navbar-toggle-collapse" is-nav>
            <b-navbar-nav class="">
              <b-nav-item href="#">Link 1</b-nav-item>
              <b-nav-item href="#">Link 2</b-nav-item>
              <b-nav-item href="#" disabled>Disabled</b-nav-item>
            </b-navbar-nav>
          </b-collapse>
          <!-- </div> -->
        </div>
      </b-navbar>

      <div>
        <b-img
          fluid
          class="image-one"
          src="https://static.wixstatic.com/media/9e3e03_4bb7950793b54f369675ce6f83605e80~mv2.png/v1/fill/w_2543,h_527,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_4bb7950793b54f369675ce6f83605e80~mv2.webp"
          style="opacity: 55%"
        ></b-img>
      </div>

      <div
        class="d-flex"
        style="background-color: rgb(1, 127, 255); height: 45px"
      >
        <b-img
          height="15"
          class="mx-auto my-auto"
          src="~/assets/most_recent_message.png"
        ></b-img>
      </div>

      <b-row>
        <b-col :cols="9"> </b-col>
        <b-col :cols="3">
          <b-img
            height="360"
            class="float-right"
            src="https://static.wixstatic.com/media/9e3e03_e3edd27a1ce84e649ecde3e589243783~mv2.jpg/v1/fill/w_589,h_361,al_t,q_80,usm_0.66_1.00_0.01/9e3e03_e3edd27a1ce84e649ecde3e589243783~mv2.webp"
          ></b-img>
        </b-col>
      </b-row>

      <div class="d-flex" style="background-color: black; height: 45px">
        <b-img
          height="15"
          class="mx-auto my-auto"
          src="~/assets/shandon_essentials.png"
        ></b-img>
      </div>

      <div class="testimonial-group bg-dark">
        <div class="row text-center">
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 1">
              <b-icon icon="chat-right-dots-fill" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 2">
              <b-icon icon="funnel" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 3">
              <b-icon icon="wallet2" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 1">
              <b-icon icon="images" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 2">
              <b-icon icon="people" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 3">
              <b-icon icon="chat-right-dots-fill" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 1">
              <b-icon icon="funnel" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 2">
              <b-icon icon="wallet2" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 3">
              <b-icon icon="images" variant="light"></b-icon>
            </p>
          </div>
          <div class="pt-2 col-4" style="height: 75px; width: 75px">
            <p class="h1" @click="selectedIcon = 1">
              <b-icon icon="people" variant="light"></b-icon>
            </p>
          </div>
        </div>
        <div id="rotatingImg1Div" v-show="selectedIcon === 1">
          <b-img
            id="rotatingImg1"
            fluid
            src="https://static.wixstatic.com/media/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.jpg/v1/fill/w_2543,h_544,al_c,q_85,usm_0.66_1.00_0.01/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.webp"
          ></b-img>
        </div>
        <div id="rotatingImg2Div" v-show="selectedIcon === 2">
          <b-img
            id="rotatingImg2"
            fluid
            src="https://static.wixstatic.com/media/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.png/v1/fill/w_2543,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.webp"
          ></b-img>
        </div>
        <div id="rotatingImg3Div" v-show="selectedIcon === 3">
          <b-img
            id="rotatingImg3"
            fluid
            src="https://static.wixstatic.com/media/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.png/v1/fill/w_2543,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.webp"
          ></b-img>
        </div>
        <div>
          <b-img
            fluid
            style="opacity: 55%"
            src="https://static.wixstatic.com/media/9e3e03_b8f4e20c76cc4280bd2c8bd7ca7ece14~mv2.jpg/v1/fill/w_1920,h_309,al_c,q_85/9e3e03_b8f4e20c76cc4280bd2c8bd7ca7ece14~mv2.webp"
          ></b-img>
        </div>
      </div>
    </div>
  </b-container>
</template>

<script lang="ts">
import Vue from 'vue'
import { BIcon } from 'bootstrap-vue'
export default Vue.extend({
  components: { BIcon },
  data: () => {
    return {
      selectedIcon: 1,
      imgSrc: [
        'https://static.wixstatic.com/media/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.jpg/v1/fill/w_2543,h_544,al_c,q_85,usm_0.66_1.00_0.01/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.webp',
        'https://static.wixstatic.com/media/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.png/v1/fill/w_2543,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.webp',
        'https://static.wixstatic.com/media/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.png/v1/fill/w_2543,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.webp',
      ],
      imgSrcTwo:
        'https://static.wixstatic.com/media/9e3e03_b8f4e20c76cc4280bd2c8bd7ca7ece14~mv2.jpg/v1/fill/w_1920,h_309,al_c,q_85/9e3e03_b8f4e20c76cc4280bd2c8bd7ca7ece14~mv2.webp',
    }
  },
  methods: {},

  created() {},
  mounted: () => {},
  computed: {},
})
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.navbar {
  background-color: black;
  height: 85px;
}

#center-nav {
  width: 40%;
}

#shandon-logo {
  height: 40px;
}

.testimonial-group > .row {
  display: block;
  overflow-x: auto;
  white-space: nowrap;
}

.testimonial-group > .row > .col-4 {
  display: inline-block;
}

@media screen and (max-width: 960px) {
  #rotatingImg1,
  #rotatingImg2,
  #rotatingImg3 {
    display: none;
  }
  #rotatingImg1Div::before {
    content: url('https://static.wixstatic.com/media/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.jpg/v1/fill/w_980,h_544,al_c,q_85,usm_0.66_1.00_0.01/9e3e03_6318cc723de24610915c5f8e89a7500a~mv2.webp');
  }
  #rotatingImg2Div::before {
    content: url('https://static.wixstatic.com/media/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.png/v1/fill/w_980,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_cc728cf70e834828af156e6afab30f51~mv2.webp');
  }
  #rotatingImg3Div::before {
    content: url('https://static.wixstatic.com/media/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.png/v1/fill/w_980,h_544,al_c,q_90,usm_0.66_1.00_0.01/9e3e03_49fa7ecfa5594c30b291b685823f76b3~mv2.webp');
  }
}
</style>
