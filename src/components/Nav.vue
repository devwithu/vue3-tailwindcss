<template>
  <div class="Nav container mx-auto my-8 grid grid-flow-col grid-cols-1 md:grid-cols-2 gap-4">
    <img :src="PorscheLogo" alt="Porsche Logo" class="w-16 mx-auto md:mx-0">
    <div class="hidden md:block">
      <div class="grid grid-flow-col grid-cols-7 gap-4 items-center   h-full ">
        <p v-for="option, optionIndex in menu" :key="optionIndex" @click="openLink(option.link)" class=" text-xs font-bold cursor-pointer" >
          {{ option.title }}
        </p>
      </div>
    </div>
    <div class="block md:hidden fixed right-8 top-8 cursor-pointer">
      <img :src="MenuIcon" alt="menu icon" class="w-8">
    </div>

  </div>
</template>

<script setup>
import PorscheLogo from '../assets/porsche_logo.png'
import MenuIcon from '../assets/menu.png'

const menu = [
  {
    title: 'Brand',
    link: ''
  }, {
    title: '718',
    link: ''
  }, {
    title: '911',
    link: ''
  }, {
    title: 'Taycan',
    link: ''
  },{
    title: 'Macan',
    link: ''
  }, {
    title: 'Panamera',
    link: ''
  }, {
    title: 'Cayenne',
    link: ''
  }
]

const openLink = (link) => {
  window.open(link)
}
</script>

