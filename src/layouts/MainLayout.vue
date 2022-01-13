<script setup>
import AuthBtn from '../components/auth/AuthBtn.vue' // eslint-disable-line no-unused-vars
</script>
<template>
  <q-layout
    view = 'hhh lpr fff'
    :container='false'
  >
    <q-header>
      <q-toolbar>
        <q-toolbar-title>
          my-blog
        </q-toolbar-title>
          <AuthBtn />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>
