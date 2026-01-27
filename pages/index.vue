<script setup lang="ts">
import BCard from '@compromis/blobby/components/card/BCard.vue'

useHead({
  htmlAttrs: {
    lang: 'ca',
  },
})

useSeoMeta({
  title: 'Sense serveis socials - Compromís',
  ogTitle: 'Sense serveis socials - Compromís',
  description: '',
  ogDescription: '',
  ogImage: 'https://sense-serveis-socials.compromis.net/images/ogimage.jpg',
  twitterCard: 'summary_large_image',
})
</script>

<template>
  <main>
    <div class="container">
      <SiteHeader>
        <SiteTitle />
      </SiteHeader>
      <section class="text text-intro">
        <h1 v-motion-fade-visible class="visually-hidden">
          Sense serveis socials
        </h1>

        <!--<Languages v-motion-slide-visible-bottom :delay="100" />-->

        <div class="questions" v-motion-slide-visible-bottom :delay="300">
          <p>
            No t’han resolt la dependència?
          </p>
          <p>
            No estàs cobrant la teua prestació per dependència?
          </p>
          <p>
            Quant de temps fa que esperes resolució del grau de discapacitat?
          </p>
          <p>
            No estan construint la residència o centre de dia del teu municipi?
          </p>
        </div>
      </section>
      </div>
      <Headlines />
      <div class="container">
      <h2 class="text-xl text-center mb-4">Dos models</h2>
      <section class="two-cols">
        <BCard padded shadow v-motion-slide-visible-bottom :delay="300">
          <h2>Compromís</h2>
          <ul class="list">
            <li><IconCheck /> Consolidar un Sistema Públic Valencià de Serveis Socials universal, de qualitat i amb les persones al centre</li>
            <li><IconCheck /> Complir amb els acords i millorar les condicions laborals per a les persones treballadores de serveis socials: cal cuidar les persones que cuiden</li>
            <li><IconCheck /> Construir centres de serveis socials públics a prop de casa, visques on visques, per a garantir la igualtat d’oportunitats</li>
            <li><IconCheck /> Gestionar amb agilitat i transparència les noves prestacions de la dependència i els canvis de grau</li>
          </ul>
        </BCard>
        <BCard padded shadow v-motion-slide-visible-bottom :delay="300">
          <h2>PP - VOX</h2>
          <ul class="list">
            <li><IconBad /> Posar els beneficis de les empreses dels seus amics per damunt dels benestar de les persones</li>
            <li><IconBad /> Desmantellar els serveis socials públics per a acabar privatitzant-los: centres tancats, ràtios més altes, menys places públiques, parar la construcció de nous equipaments</li>
            <li><IconBad /> Ocultar de forma deliberada les llistes d’espera de la dependència i no pagar els retards en el canvi de grau</li>
            <li><IconBad /> Degradar les condicions laborals de les persones treballadores dels serveis socials</li>
          </ul>
        </BCard>
      </section>
      <div class="text text-intro">
        <BCard padded shadow v-motion-slide-visible-bottom :delay="300">
            <ContactForm />
        </BCard>
      </div>
    </div>
    <Share>
      <template #title>Fes-ne difusió!</template>
      <p>Comparteix aquesta pàgina amb les teues amistats.</p>
    </Share>
  </main>
</template>
