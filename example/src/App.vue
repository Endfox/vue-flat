<template>
  <div id="app">
    <Title text="Vue Flat" />
    <tag-component text="example text"></tag-component>
    <btn />
    <List :list="lista" />
    <btnGosh text="Submit" :border=true />
  </div> 
</template>

<script>
import { tagComponent, btn, List,Title,btnGosh } from '../../src/index'

export default {
  name: 'app',
  data: () => ({
    lista:['leo', 'yami', 'tibe']
  }),
  components: {
    tagComponent,
    btn,
    List,
    Title,
    btnGosh
  }
}
</script>

<style>
  #app{
    height:1500px;
    background:black;
  }
</style>