<template>
  <div id="app">
    <Sidebar/>
    <router-view/>
  </div>
</template>

<script>
import Sidebar from './components/layout/sidebar/Sidebar'

export default {
  name: 'App',

  components: {
    Sidebar,
  }
}
</script>