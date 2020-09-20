<template>
  <div class="home">
    <div v-for="i in 50" :key="i">
      <header>Section {{ i }}</header>

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, provident nisi reiciendis at fugit autem repellat blanditiis eos dolorem. Tenetur distinctio nihil ullam laudantium repudiandae. Consequatur necessitatibus quod dolorum est.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>
