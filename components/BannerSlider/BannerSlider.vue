<template>
  <div class="banner-wrap">
    <div class="carousel" v-if="loaded">
      <slick
        ref="slider"
        :options="slickOptions"
        @afterChange="handleAfterChange"
      >
        <div class="slide" v-for="(item,index) in data" :key="index">
          <div class="inner">
            <v-container>
              <v-row>
                <v-col sm="7" lg="6" cols="12">
                  <div class="text">
                    <h4 class="text-h4">{{item.title}}</h4>
                    <h5 class="text-h5">{{ item.subtitle }}</h5>
                  </div>
                </v-col>
              </v-row>
            </v-container>
            <div class="img">
              <img :src="item.img" alt="illustration" />
            </div>
          </div>
        </div>
      </slick>
    </div>
    <hidden point="mdDown">
      <v-container class="max-md">
        <nav class="slide-nav">
          <v-btn
            :class="{ active: currentSlide === 0 }"
            @click="gotoSlide(0)"
            text
          >
            <strong>First Slide</strong>
            this is first slide
          </v-btn>
          <v-divider class="divider" vertical inset />
          <v-btn
            :class="{ active: currentSlide === 1 }"
            @click="gotoSlide(1)"
            text
          >
            <strong>Second Slide</strong>
            this is second slide
          </v-btn>
          <v-divider class="divider" vertical inset />
          <v-btn
            :class="{ active: currentSlide === 2 }"
            @click="gotoSlide(2)"
            text
          >
            <strong>Third Slide</strong>
           this is third slide :)
          </v-btn>
        </nav>
      </v-container>
    </hidden>
  </div>
</template>

<style scoped lang="scss">
@import './slider-styles';
</style>

<script>
import Hidden from '../Hidden';
import {data } from "@/data/carousel"

export default {
  components: {
    Hidden,
    Slick: () => import('vue-slick')
  },
  data() {
    return {
      data,
      loaded: false,
      currentSlide: 0,
      slickOptions: {
        dots: false,
        arrows: false,
        slidesToShow: 1,
        infinite: true,
        autoplay: true,
        autoplaySpeed: 1500,
        responsive: [
          {
            breakpoint: 800,
            settings: {
              dots: true
            }
          }
        ]
      }
    }
  },
  mounted() {
    this.loaded = true
    // console.log($t('starter'))
  },
  methods: {
     getImgUrl(image) {
    // var images = require.context('../assets/', false, /\.png$/)
    // return images('./' + image )
  },
    handleAfterChange(event, slick, currentSlide) {
      this.currentSlide = currentSlide
    },
    gotoSlide(index) {
      this.$refs.slider.goTo(index)
    }
  }
}
</script>
