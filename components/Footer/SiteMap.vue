<template>
  <footer class="footer">
    <v-container>
      <v-row>
        <v-col
          class="pa-4 px-lg-10"
          md="3"
          cols="12"
        >
          <logo type="portrait" />
          <p v-if="isDesktop" class="body-2 text-center">
            &copy;&nbsp;
            {{ brand.starter.footerText }}
          </p>
        </v-col>
        <v-col
          class="pa-4"
          md="6"
          cols="12"
        >
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2000.1584053239424!2d10.762135016095936!3d59.91291838186684!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46416e5fa540d387%3A0xf5da575472c100c2!2sT%C3%B8yengata%202%2C%200190%20Oslo!5e0!3m2!1sen!2sno!4v1636639953364!5m2!1sen!2sno" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </v-col>
        <v-col
          md="3"
          cols="12"
          class="pa-4"
        >
          <div class="socmed">
            <v-btn
              text
              icon
              class="button"
            >
              <a href="https://www.facebook.com/Changegroup" target="_blank"><span class="ion-social-facebook icon" /> </a>
            </v-btn>
            <v-btn
              text
              icon
              class="button"
            >
              <a href="https://www.instagram.com/changegroupno/?hl=en" target="_blank"> <span class="ion-social-instagram icon" /></a>
            </v-btn>
            <v-btn
              text
              icon
              class="button"
            >
              <a href="https://www.linkedin.com/company/change-marketing-as/?originalSubdomain=no" target="_blank"><span class="ion-social-linkedin icon" /></a>
            </v-btn>
          </div>
          <p v-if="isMobile" class="body-2 text-center">
            &copy;&nbsp;
            {{ brand.starter.footerText }}
          </p>
        </v-col>
      </v-row>
    </v-container>
  </footer>
</template>

<style scoped lang="scss">
@import './footer-sitemap';
</style>

<script>
import Logo from '../Logo'
import brand from '~/static/text/brand'

export default {
  components: {
    Logo
  },
  data: () => ({
    brand: brand,
    lang: 'en',
    footers: [
      {
        title: 'company',
        description: ['Team', 'History', 'Contact us', 'Locations'],
        link: ['#team', '#history', '#contact-us', '#locations']
      },
      {
        title: 'resources',
        description: [
          'Resource',
          'Resource name',
          'Another resource',
          'Final resource'
        ],
        link: [
          '#resource',
          '#resource-name',
          '#another-resource',
          '#final-resource'
        ]
      },
      {
        title: 'legal',
        description: ['Privacy policy', 'Terms of use'],
        link: ['#privacy-policy', '#terms-of-use']
      }
    ]
  }),
  mounted() {
    this.lang = this.$i18n.locale
  },
  computed: {
    langList: function() {
      const list = []
      this.$i18n.locales.map(item => {
        list.push({ text: this.$t('common.' + item.code), value: item.code })
      })
      return list
    },
    isMobile() {
      const smDown = this.$store.state.breakpoints.smDown
      return smDown.indexOf(this.$mq) > -1
    },
    isDesktop() {
      const mdUp = this.$store.state.breakpoints.mdUp
      return mdUp.indexOf(this.$mq) > -1
    }
  },
  methods: {
    switchLang: function(val) {
      this.$i18n.setLocale(val)
    }
  }
}
</script>
