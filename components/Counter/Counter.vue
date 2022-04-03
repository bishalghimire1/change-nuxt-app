<template>
  <div class="counter-wrap" :class="{ dark: dark }">
    <div id="watched_counter" />
    <v-container class="max-md">
      <v-row
        align="center"
        justify="center"
        class="root"
      >
        <v-col sm="4">
          <div class="counter-item">
            <span class="icon ion-email" />
            <div class="text">
              <!-- <h4 class="display-1" v-if="loaded">
                +
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 123,
                    options: { duration: 1 }
                  }"
                />
              </h4> -->
              <a class="white--text" href="mailto:kontakt@changegroup.no">kontakt@changegroup.no</a>
            </div>
          </div>
        </v-col>
        <v-col sm="4">
          <div class="counter-item">
            <span class="icon ion-android-call" />
            <div class="text">
              <!-- <h4 class="display-1" v-if="loaded">
                +
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 456,
                    options: { duration: 1 }
                  }"
                />
              </h4> -->
              <h6 class="use-text-subtitle2">+47 483 57 777</h6>
            </div>
          </div>
        </v-col>
        <v-col sm="4">
          <div class="counter-item">
            <span class="icon ion-ios-world-outline" />
            <div class="text">
              <!-- <h4 class="display-1" v-if="loaded">
                $
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 789,
                    options: { duration: 1 }
                  }"
                />
              </h4> -->
              <h6 class="use-text-subtitle2">Tøyengata 2, 0190 Oslo</h6>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
@import './counter-style';
</style>

<script>
export default {
  data: () => ({
    loaded: false
  }),
  mounted() {
    this.loaded = true
  },
  props: {
    dark: {
      type: Boolean,
      default: false
    }
  }
}
</script>
