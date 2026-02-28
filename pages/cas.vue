<script setup lang="ts">
import BCard from '@compromis/blobby/components/card/BCard.vue'

useHead({
  htmlAttrs: {
    lang: 'es',
  },
})

useSeoMeta({
  title: 'Sin servicios sociales - Compromís',
  ogTitle: 'Sin servicios sociales - Compromís',
  description: '¿No te han resuelto la dependencia? ¿Estás esperando plaza de centro de día o residencia desde hace más de 6 meses?',
  ogDescription: '¿No te han resuelto la dependencia? ¿Estás esperando plaza de centro de día o residencia desde hace más de 6 meses?',
  ogImage: 'https://sense-serveis-socials.compromis.net/images/ogimage.jpg',
  twitterCard: 'summary_large_image',
  keywords: 'servicios sociales, dependencia, discapacidad, residencias, centros de día, listas de espera, Compromís',
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
          Sin servicios sociales
        </h1>

        <Languages v-motion-slide-visible-bottom :delay="100" />

        <div class="questions" v-motion-slide-visible-bottom :delay="300">
          <p>
            ¿No te han resuelto la dependencia?
          </p>
          <p>
            ¿Estás esperando plaza de centro de día o residencia desde hace más de 6 meses?
          </p>
          <p>
            ¿Cuánto tiempo llevas esperando la resolución del grado de discapacidad?
          </p>
          <p>
            ¿No están construyendo la residencia o centro de día de tu municipio?
          </p>
          <p>
            ¿Como profesional, el sistema se está desbordando? ¿Cómo te afecta?
          </p>
        </div>
      </section>
      </div>
      <Headlines />
      <div class="container">
      <h2 class="text-xl text-center mb-4">Dos modelos</h2>
      <section class="two-cols">
        <BCard padded shadow v-motion-slide-visible-bottom :delay="300">
          <h2>Compromís</h2>
          <ul class="list">
            <li><IconCheck /> Consolidar un Sistema Público Valenciano de Servicios Sociales universal, de calidad y con las personas en el centro</li>
            <li><IconCheck /> Cumplir con los acuerdos y mejorar las condiciones laborales para las personas trabajadoras de servicios sociales: hay que cuidar a las personas que cuidan</li>
            <li><IconCheck /> Construir centros de servicios sociales públicos cerca de casa, vivas donde vivas, para garantizar la igualdad de oportunidades</li>
            <li><IconCheck /> Gestionar con agilidad y transparencia las nuevas prestaciones de la dependencia y los cambios de grado</li>
          </ul>
        </BCard>
        <BCard padded shadow v-motion-slide-visible-bottom :delay="300">
          <h2>PP - VOX</h2>
          <ul class="list">
            <li><IconBad /> Poner los beneficios de las empresas de sus amigos por encima del bienestar de las personas</li>
            <li><IconBad /> Desmantelar los servicios sociales públicos para acabar privatizándolos: centros cerrados, ratios más altas, menos plazas públicas, parar la construcción de nuevos equipamientos</li>
            <li><IconBad /> Ocultar de forma deliberada las listas de espera de la dependencia y no pagar los retrasos en el cambio de grado</li>
            <li><IconBad /> Degradar las condiciones laborales de las personas trabajadoras de los servicios sociales</li>
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
      <template #title>¡Difúndelo!</template>
      <p>Comparte esta página con tus amistades.</p>
    </Share>
  </main>
</template>
