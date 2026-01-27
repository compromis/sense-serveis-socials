<template>
  <BCard padded shadow class="headline-wrapper">
    <a
      ref="card"
      :href="url"
      target="_blank"
      rel="noopener"
      class="headline"
      :style="{
        '--rotate': `${rotateTo}deg`,
      }"
    >
      <img :src="source[1]" :alt="source[0]" class="logo" />
      <h4 class="heading">
        <slot />
      </h4>
    </a>
  </Bcard>
</template>

<script lang="ts" setup>
const props = defineProps({
  source: {
    type: Array,
    required: true
  },
  url: {
    type: String,
    required: true
  }
})

const { $gsap } = useNuxtApp()

const card = ref(null)
const rotateTo = useState(`rotate-from-${props.url}`, () => Math.random() * 4 - 2)
const rotateFrom = useState(`rotate-to-${props.url}`, () => Math.random() * 10 - 8)

onMounted(() => {
  $gsap.from(card.value, {
    opacity: 0,
    y: 75,
    rotate: rotateFrom.value,
    scale: 0.85,
    ease: 'Elastic.easeOut',
    duration: 1.25,
    scrollTrigger: {
      trigger: card.value,
      start: 'top bottom',
      toggleActions: "restart none none reverse"
    },
  })
})

</script>

<style lang="scss" scoped>
.headline {
  rotate: var(--rotate);
  display: block;
  background: white;
  padding: 1rem;
  color: var(--green-dark);
  width: 23vw;
  border-radius: 1rem;
  margin-right: 2rem;
}

.logo {
  height: 1rem;
}

.heading {
  font-family: "Instrument Serif", serif;
  font-size: 3rem;
}

.headline-wrapper {
  transition: .25s ease;

  &:hover {
    scale: 1.05;
    rotate: -1deg;
  }
}
</style>