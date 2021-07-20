<template>
  <div class="Stats bg-cover bg-no-repeat bg-bottom" :style="`background-image:url(${PorscheBackground}); height: 450px; `">
    <div class="w-full h-full bg-customBlue opacity-75 absolute z-0">
      <div class="Stats-Component z-50 relative">
        <p class="text-white">some test</p>
      </div>
    </div>
  </div>
  <StatsCard></StatsCard>
</template>

<script setup>
import StatsCard from './elements/stats/StatsCard.vue'
import PorscheBackground from '../assets/2020-porsche.jpeg'

</script>
