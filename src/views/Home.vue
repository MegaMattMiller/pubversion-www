<template>
  <div class="home">
    <div id="termynal" data-termynal data-ty-type-delay="40" data-ty-line-delay="700">
      <span data-ty="input">pub global activate pubversion</span>
      <span data-ty>Resolving dependencies...</span>
      <span data-ty>Activated pubversion 1.0.0</span>
      <span data-ty="input">pubversion major</span>
      <span data-ty>example_lib upgraded from 1.0.2 to 2.0.0</span>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: "home",
  components: {}
};
</script>


