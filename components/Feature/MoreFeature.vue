<template>
  <div class="feature-more">
    <v-container>
      <u-animate-container>
        <v-row id="feature1">
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="fadeInLeft"
                duration="0.6s"
              >
                <h3 class="title-app display-2">B2B</h3>
              </u-animate>
              <u-animate
                name="fadeInLeft"
                delay="0.3s"
                duration="0.6s"
              >
                <p class="text">
                  Vi tilbyr salg i tvers av bedriftene gjennom Zoomplus. Der vi tilbyr store og små bedrifter hjelp med markedsføring.
                </p>
              </u-animate>
            </div>
          </v-col>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="zoomIn"
                delay="0.3s"
                duration="0.6s"
              >
                <div class="deco1" />
              </u-animate>
              <u-animate
                name="fadeInRight"
                delay="0.5s"
                duration="0.6s"
              >
                <figure class="img">
                  <img
                    src="/images/home/b2b.png"
                    alt="img"
                  >
                </figure>
              </u-animate>
            </div>
          </v-col>
        </v-row>
      </u-animate-container>
      <u-animate-container>
        <v-row>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="zoomIn"
                delay="0.3s"
                duration="0.6s"
              >
                <div class="deco1" />
              </u-animate>
              <u-animate
                name="fadeInLeft"
                delay="0.5s"
                duration="0.6s"
              >
                <figure class="img">
                  <img
                    src="/images/home/responsive.png"
                    alt="img"
                  >
                </figure>
              </u-animate>
            </div>
          </v-col>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="fadeInLeft"
                duration="0.6s"
              >
                <h3 class="title-app display-2">IT Utvikling</h3>
              </u-animate>
              <u-animate
                name="fadeInRight"
                delay="0.5s"
                duration="0.6s"
              >
                <p class="text">
                  Vi tilbyr tjenester innenfor app utvikling og drift av nettsider.
                </p>
              </u-animate>
            </div>
          </v-col>
        </v-row>
      </u-animate-container>
           <u-animate-container>
        <v-row id="feature1">
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="fadeInLeft"
                duration="0.6s"
              >
                <h3 class="title-app display-2">Media Produksjon</h3>
              </u-animate>
              <u-animate
                name="fadeInLeft"
                delay="0.3s"
                duration="0.6s"
              >
                <p class="text">
                  Vi jobber med å utvikle designen til både nye og eldre selskap i markedet. Vi fokuserer på å dekke kundens behov ved hjelp av vår profesjonelle erfaring innad i medieproduksjon.
                </p>
              </u-animate>
            </div>
          </v-col>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="zoomIn"
                delay="0.3s"
                duration="0.6s"
              >
                <div class="deco1" />
              </u-animate>
              <u-animate
                name="fadeInRight"
                delay="0.5s"
                duration="0.6s"
              >
                <figure class="img">
                  <img
                    src="/images/home/media.png"
                    alt="img"
                  >
                </figure>
              </u-animate>
            </div>
          </v-col>
        </v-row>
      </u-animate-container>
      <u-animate-container>
        <v-row>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="zoomIn"
                delay="0.3s"
                duration="0.6s"
              >
                <div class="deco1" />
              </u-animate>
              <u-animate
                name="fadeInLeft"
                delay="0.5s"
                duration="0.6s"
              >
                <figure class="img">
                  <img
                    src="/images/home/slider_2.jpeg"
                    alt="img"
                  >
                </figure>
              </u-animate>
            </div>
          </v-col>
          <v-col
            md="6"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item">
              <u-animate
                name="fadeInLeft"
                duration="0.6s"
              >
                <h3 class="title-app display-2">Dørsalg</h3>
              </u-animate>
              <u-animate
                name="fadeInRight"
                delay="0.5s"
                duration="0.6s"
              >
                <p class="text">
                  Gjennom vår lange erfaring innad i dørsalg tilbyr vi dørsalg både for virksomheter og for ansatte.
                </p>
              </u-animate>
            </div>
          </v-col>
        </v-row>
      </u-animate-container>
      <v-container
        fluid
        class="pa-0"
      >
        <!-- <v-row align="center">
          <v-col
            cols="12"
            sm="12"
          >
            <div class="text-center">
              <div class="my-2">
                <v-btn
                  x-large
                  color="success"
                  dark
                >
                  Se alle tjenester
                </v-btn>
              </div>
            </div>
          </v-col>
        </v-row> -->
      </v-container>
      <v-divider
      inset
      ></v-divider>
      <u-animate-container>
        <v-row>
          <v-col
            md="12"
            class="px-6"
            cols="12"
          >
            <div v-if="loaded" class="feature-item last text-center">
              <u-animate
                name="fadeInUp"
                duration="0.6s"
              >
                <h3 class="title-app display-2">Kontakt Oss</h3>
              </u-animate>
              <u-animate
                name="fadeInUp"
                duration="0.6s"
                delay="0.3s"
              >
                <p class="text">
                  Ring oss eller ring oss hvis du er interessert i å besøke oss.
                </p>
              </u-animate>
              <u-animate
                name="zoomIn"
                duration="0.6s"
                delay="0.3s"
              >
                <div class="deco2" />
              </u-animate>
              <u-animate
                name="fadeInUp"
                duration="0.6s"
                delay="0.5s"
              >
                <figure class="img-full">
                  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2000.1584053239424!2d10.762135016095936!3d59.91291838186684!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46416e5fa540d387%3A0xf5da575472c100c2!2sT%C3%B8yengata%202%2C%200190%20Oslo!5e0!3m2!1sen!2sno!4v1636554025191!5m2!1sen!2sno" width="100%" height="400" style="border:0;" class="map_border" loading="lazy"></iframe>
                </figure>
              </u-animate>
            </div>
          </v-col>
        </v-row>
      </u-animate-container>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
@import './feature-styles';
.map_border{
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
}
</style>

<script>
import imgAPI from '~/static/images/imgAPI'

export default {
  data() {
    return {
      imgAPI,
      loaded: false
    }
  },
  mounted() {
    this.loaded = true
  }
}
</script>
