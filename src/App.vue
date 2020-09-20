<template>
  <div id="app">
    <BaseLayout>
      <router-view/>
    </BaseLayout>
  </div>
</template>

<script>
import BaseLayout from './components/layout/base-layout/BaseLayout'

export default {
  name: 'App',

  components: {
    BaseLayout,
  }
}
</script>