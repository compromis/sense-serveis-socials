<template>
  <Vue3Marquee class="headlines" :gap="20" :duration="100">
    <Headline :source="['Europa Press', europapress]" url="https://www.europapress.es/comunitat-valenciana/noticia-comunitat-valenciana-cuatro-ccaa-mas-aumentan-lista-espera-dependencia-218-20250707142734.html">
      La Comunitat Valenciana, entre las cuatro CCAA que <Annotated immediate>ás aumentan su lista de espera</Annotated> de dependencia: un 21,8%
    </Headline>

    <Headline :source="['eldiario.es', eldiario]" url="https://www.eldiario.es/comunitat-valenciana/jueza-dana-investiga-viviendas-generalitat-pegadas-barranco-poyo-murieron-ocho-ancianos_1_12824991.html">
      La jueza de la dana investiga las viviendas de la Generalitat pegadas al barranco del Poyo donde murieron ocho ancianos
    </Headline>

    <Headline :source="['Levante', levante]" url="https://www.levante-emv.com/comunitat-valenciana/2025/07/24/compromis-exige-abra-centro-salud-120029923.html">
      Compromís exige <Annotated immediate>que se abra el centro de salud mental</Annotated> listo y equipado desde hace más de dos años en Bétera
    </Headline>

    <Headline :source="['Levante', levante]" url="https://www.levante-emv.com/comunitat-valenciana/2025/03/25/varapalo-dana-gestion-servicios-sociales-115655773.html">
      Varapalo del Síndic de Greuges por la dana y la gestión de Servicios Sociales
    </Headline>

    <Headline :source="['Valencia Plaza', valenciaplazaLogo]" url="https://valenciaplaza.com/valenciaplaza/comunitat-valenciana1/entidades-de-servicios-sociales-de-la-comunitat-denuncian-la-precariedad-y-privatizacion-del-sector-y-reclaman-mejoras">
      Entidades de servicios sociales de la Comunitat denuncian la <Annotated immediate>"precariedad y privatización"</Annotated> del sector y reclaman mejoras
    </Headline>

    <Headline :source="['Diari La Veu', diarilaveu]" url="https://www.diarilaveu.cat/societat/la-paralisi-del-pla-convivint-suposa-perdre-136-milions-en-fons-europeus-582175/">
      La paràlisi del Pla Convivint suposa <Annotated immediate>perdre 136 milions</Annotated> en fons europeus
    </Headline>

    <Headline :source="['La Ser', ser]" url="https://cadenaser.com/comunitat-valenciana/2025/12/12/ccoo-alerta-de-que-el-sistema-de-atencion-a-la-dependencia-sufre-un-retroceso-por-las-decisiones-del-consell-radio-elche/">
      CCOO alerta de que el sistema de atención a <Annotated immediate>la dependencia sufre un retroceso</Annotated> por las decisiones del Consell
    </Headline>
  </Vue3Marquee>
</template>

<script lang="ts" setup>
import europapress from '~/assets/images/headlines/europapress.png'
import eldiario from '~/assets/images/headlines/eldiario.svg'
import levante from '~/assets/images/headlines/levante.svg'
import valenciaplazaLogo from '~/assets/images/headlines/valenciaplaza.svg'
import ser from '~/assets/images/headlines/ser.svg'
import diarilaveu from '~/assets/images/headlines/diarilaveu.svg'
</script>
