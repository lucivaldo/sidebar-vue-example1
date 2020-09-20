<template>
  <div class="base-layout">
    <Sidebar/>
    <Navbar/>

    <main class="main"><slot/></main>
  </div>
</template>

<script>
import Sidebar from '../sidebar/Sidebar'
import Navbar from '../navbar/Navbar'

export default {
  name: 'BaseLayout',

  components: {
    Sidebar,
    Navbar,
  }
}
</script>

<style lang="scss" scoped>
.base-layout {
  height: 100%;
}
</style>