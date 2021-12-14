<template>
  <q-page class="flex column q-pa-md">
    <span class="text-h1">Headline 1</span>
    <span class="text-h2">Headline 2</span>
    <span class="text-h3">Headline 3</span>
    <span class="text-h4">Headline 4</span>
    <span class="text-h5">Headline 5</span>
    <span class="text-h6">Headline 6</span>

    <span class="text-subtitle1">Subtitle 1</span>
    <span class="text-subtitle2">Subtitle 2</span>

    <q-separator />
    <p class="text-body1">Quis occaecat irure labore aliqua anim dolore Lorem</p>
    <p class="text-body2">Lorem ipsum blablabla bla bla bla bla bla bla bla</p>
    <q-separator />

    <span class="text-weight-thin">Veniam esse ex cillum elit</span>
    <span class="text-weight-light">Mollit proident esse est dolor</span>
    <span class="text-weight-regular">Culpa velit ullamco sunt aliqua enim</span>
    <span class="text-weight-medium">Commodo mollit anim elit ea aliqua</span>
    <span class="text-weight-bold">Elit voluptate reprehenderit sint ut fugiat sunt sit</span>
    <span class="text-weight-bolder">Velit mollit dolore deserunt elit reprehenderit</span>

    <q-btn
      color="primary"
      :label="sideMenuOpen ? 'Cerrar menú lateral' : 'Abrir menú lateral'"
      class="q-mt-md"
      @click="toggleSideMenu"
    />

  </q-page>
</template>

<script>

import { defineComponent } from 'vue'
import useUI from '../composables/useUI'

export default defineComponent({
  name: 'Typography',

  setup () { 

    const { sideMenuOpen, toggleSideMenu } = useUI() 

    return {
      sideMenuOpen,
      toggleSideMenu,
    }
  }
})

</script>
