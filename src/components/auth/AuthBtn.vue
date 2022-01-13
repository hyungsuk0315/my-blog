<script lang='ts'>
import { initializeApp } from 'firebase/app'
import firebaseConfig from '../../../firebaseConfig.js'
import {
  getAuth,
  GoogleAuthProvider,
  connectAuthEmulator,
  signInWithPopup
} from 'firebase/auth'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'AuthBtn',
  setup () {
    console.log('sdfasf')
    initializeApp(firebaseConfig)
    const auth = getAuth()
    connectAuthEmulator(auth, 'http://localhost:9099')
    auth.useDeviceLanguage()
    const provider = new GoogleAuthProvider()
    return { auth, provider, signInWithPopup }
  }
})
</script>

<template>
  <button>sdjfalskf</button>
</template>
