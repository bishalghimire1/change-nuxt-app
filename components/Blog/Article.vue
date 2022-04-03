<template>
  <article class="blog-content">
    <h4 class="text-h4 title-blog">HVORDAN FOREGÅR EN GOD ANSETTELSESPROSESS
</h4>
    <time class="caption">June 19, 2020 - Change Group</time>
    <figure class="image-blog">
      <img src="https://source.unsplash.com/random" alt="change group" />
    </figure>
    <p>En god ansettelsesprosess innebærer blant annet å ansette den kandidaten som vil passe
best til stillingen og bedriften. For å lykkes med dette er rekruttering tilpasset bedriften
nøkkelen. Målet er å bygge et team som motiverer og samarbeider godt. Dette skaper
suksess for både bedriften og den ansatte.</p>
    <p>En grundig rekrutteringsprosess er avgjørende både for bedriften og kandidaten. Det er flere
faktorer som avgjør om en kandidat vil passe til stillingen og arbeidsstedet. En god CV og
personlig kjemi er ikke det eneste som er avgjørende ved rekruttering. Med en grundig
rekrutteringsprosess vil både kandidat og arbeidsplassen få en ansatt som vil yte sitt beste
og vil bli værende i bedriften.</p>
    <figure class="image-blog">
      <img src="https://source.unsplash.com/random" alt="change group" />
    </figure>
    <strong>Donec ullamcorper nulla non metus auctor fringilla. Nulla vitae elit libero, a  pharetra augue.</strong>
    <ol>
      <li>Kandidater som har undersøkt bedriften og satt seg inn i stillingen som er utlyst på
forhånd, viser iver for stillingen og selskapet.</li>
      <li>Ærlighet; en kandidat som kjenner seg selv, både på en positiv og mindre positiv måte sier mye om kandidaten.
</li>
      <li>En god flyt i samtalen gir et inntrykk og et godt grunnlag for å se om kandidaten er
den bedriften ser etter.</li>
<li>Grundig bakgrunnssjekk av kandidaten kan gi en indikasjon på inntrykket som
kandidaten gir av seg selv i rekrutteringsprosessen.</li>
<li>Kandidatens kompetanse, tidligere erfaringer og arbeid kan gi en indikasjon på om
ovennevnte punkter stemmer med inntrykket kandidaten har gitt og er liten pekepinn
både for rekrutterer og kandidaten på hvordan kandidaten vil passe inn i bedriften.</li>
    </ol>

  </article>
</template>

<style scoped lang="scss">
@import './blog-style.scss';
</style>

<script>
import Form from '../Comment/Form'
import Item from '../Comment/Item'

export default {
  components: {
    'comment-item': Item,
    'comment-form': Form
  },
  data() {
    return {
      comments: [
        {
          name: 'John Doe',
          avatar: '/images/avatars/pp_boy4.svg',
          date: '13 Jan 2020',
          comment:
            'Maecenas nisl libero, tincidunt id odio id, feugiat vulputate quam. Vestibulum feugiat rhoncus metus. In non erat et ipsum molestie porta sit amet ut felis. Vestibulum a massa vestibulum, gravida odio id, fringilla ipsum.'
        },
        {
          name: 'John Doe',
          avatar: '/images/avatars/pp_boy4.svg',
          date: '13 Jan 2020',
          comment:
            'Maecenas nisl libero, tincidunt id odio id, feugiat vulputate quam. Vestibulum feugiat rhoncus metus. In non erat et ipsum molestie porta sit amet ut felis. Vestibulum a massa vestibulum, gravida odio id, fringilla ipsum.'
        },
        {
          name: 'John Doe',
          avatar: '/images/avatars/pp_boy4.svg',
          date: '13 Jan 2020',
          comment:
            'Maecenas nisl libero, tincidunt id odio id, feugiat vulputate quam. Vestibulum feugiat rhoncus metus. In non erat et ipsum molestie porta sit amet ut felis. Vestibulum a massa vestibulum, gravida odio id, fringilla ipsum.'
        },
        {
          name: 'John Doe',
          avatar: '/images/avatars/pp_boy4.svg',
          date: '13 Jan 2020',
          comment:
            'Maecenas nisl libero, tincidunt id odio id, feugiat vulputate quam. Vestibulum feugiat rhoncus metus. In non erat et ipsum molestie porta sit amet ut felis. Vestibulum a massa vestibulum, gravida odio id, fringilla ipsum.'
        }
      ]
    }
  },
  computed: {
    isMobile() {
      const xsDown = this.$store.state.breakpoints.xsDown
      return xsDown.indexOf(this.$mq) > -1
    }
  }
}
</script>
