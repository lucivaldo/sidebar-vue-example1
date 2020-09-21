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

// Posicionamento do conteúdo principal
.main {
  margin-left: calc(2 * 1rem + 2rem);
  margin-top: 4rem;
  transition: margin-left .3s;
}

.nav--expand .main {
  margin-left: 15rem;
}

.subnav--active .main {
  margin-left: calc(2 * 1rem + 2rem + 20rem);
}

.nav--expand.subnav--active .main {
  margin-left: calc(15rem + 20rem);
}

.nav--expand.subnav--active.subnav--shrink .main {
  margin-left: calc(15rem);
}

.subnav--active.subnav--shrink .main {
  margin-left: calc(2 * 1rem + 2rem);
}
</style>