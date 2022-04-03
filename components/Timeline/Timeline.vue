<template>
<div>
<h2 class="text-center title-app display-2 mb-10 ">Verdier</h2>
  <v-timeline :dense="$vuetify.breakpoint.smAndDown">

    <v-timeline-item
      color="purple lighten-2"
      fill-dot
      right
    >
      <v-card>
        <v-card-title class="purple lighten-2">
          <v-icon
            dark
            size="42"
            class="mr-4"
          >
            mdi-forward
          </v-icon>
          <h2 class="text-h4 white--text font-weight-light">
            Fremoverlente
          </h2>
        </v-card-title>
        <v-container>
          <v-row>
            <v-col
              cols="12"
              md="10"
            >
I et ungt og dynamisk arbeidsmiljø mener vi det er viktig å ha en fremoverlent tilnærming til salgsprosesser og arbeidsoppgaver. I dette legger vi at arbeidstakere selv har mulighet for å ta initiativ og fatte besluttninger, noe som gir rom for feilsteg og læring. En fremoverlent kultur på arbeidsplassen skal være med på skape karakter, arbeidstempo og innsatsvilje.

            </v-col>
            <v-col
              class="hidden-sm-and-down text-right"
              md="2"
            >
              <v-icon size="64">
                mdi-calendar-text
              </v-icon>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-timeline-item>

    <v-timeline-item
      color="amber lighten-1"
      fill-dot
      left
      small
    >
      <v-card>
        <v-card-title class="amber lighten-1 justify-end">
          <h2 class="text-h4 mr-4 white--text font-weight-light">
            Kompetente
          </h2>
          <v-icon
            dark
            size="42"
          >
            mdi-anchor
          </v-icon>
        </v-card-title>
        <v-container>
          <v-row>
            <v-col
              cols="12"
              md="10"
            >
              Vi er alltid på søken etter å forbedre kompetansenivået vårt som organisasjon, så vel som på individ nivå. Filosofien “sammen står vi sterke” skal sette rammer for teoretiske og praktiske utfordringer. Det er viktig for oss at en arbeidshverdag i Change group gir grobunn for læring og kompetanseløft, noe som gir våre kunder og samarbeidspartnere merverdi.
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-timeline-item>

    <v-timeline-item
      color="cyan lighten-1"
      fill-dot
      right
    >
      <v-card>
        <v-card-title class="cyan lighten-1">
          <v-icon
            class="mr-4"
            dark
            size="42"
          >
            mdi-chevron-triple-right
          </v-icon>
          <h2 class="text-h4 white--text font-weight-light">
            Løsningsorienterte
          </h2>
        </v-card-title>
        <v-container>
          <v-row>
            <v-col
              cols="12"
              md="10"
            >
              Med oppstart og SMB markedet som vårt hovedsegment faller det seg naturlig og ha en løsningsorientert tilnærming til hvordan et kundeforhold skal opprettholdes både når det gjelder arbeidsflyt og belastning for våre tjenester. Sammen skal vi i felleskap finne de beste og mest bærekraftige løsningene for et sunt og fruktbart samarbeid på lang sikt.
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</div>
</template>