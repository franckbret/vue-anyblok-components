<template>
  <div class="home container">
    <img alt="Vue logo" src="../assets/vue-logo.png">
    <img alt="AnyBlok logo" src="../assets/anyblok-logo.png">
    <HelloWorld msg="Welcome to vue-anyblok-components"/>
    <section class="section">
      <ComponentA />
      <ComponentA />
      <ComponentA />
    </section>
    <section class="section">
      <ComponentB v-on:click="logInput" />
      <ComponentB v-on:click="logInput">Plop</ComponentB>
    </section>
    <section class="section">
      <b-taglist class="is-centered">
          <b-tag type="is-info">First</b-tag>
          <b-tag type="is-primary">Second</b-tag>
          <b-tag type="is-dark">Third</b-tag>
          <b-tag type="is-light">Fourth</b-tag>
          <b-tag type="is-info">Fifth</b-tag>
      </b-taglist>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import ComponentA from '@/components/ComponentA.vue'
import ComponentB from '@/components/ComponentB.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    ComponentA,
    ComponentB
  },
  methods: {
    logInput (value) {
      console.log('logInput with value from child component: ' + value)
    }
  }
}
</script>
