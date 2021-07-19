<template>
  <div>
    <Nav></Nav>
    <MainHeader></MainHeader>
    <Presentation oriented="left"></Presentation>
    <Presentation oriented="right"></Presentation>
    <Stats></Stats>
    <Tabs></Tabs>
    <Footer></Footer>
  </div>
</template>

<script setup>
import { Nav, MainHeader, Presentation, Stats, Tabs, Footer } from '../components'
</script>
