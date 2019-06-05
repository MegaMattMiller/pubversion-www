<template>
  <div class="home">
    <div class="header">
      <h1 class="main-text">pubversion</h1>
      <h6 class="body-text">A Dart command-line tool for easily incrementing package version numbers</h6>
    </div>
    
    <div class="terminal">
      <div id="termynal" data-termynal data-ty-type-delay="40" data-ty-line-delay="700">
        <span data-ty="input">pub global activate pubversion</span>
        <span data-ty>Resolving dependencies...</span>
        <span data-ty>Activated pubversion 1.0.0</span>
        <span data-ty="input">pubversion major</span>
        <span data-ty>example_lib upgraded from 1.0.2 to 2.0.0</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  components: {},
  mounted() {
    let termynalScript = document.createElement("script");
    termynalScript.setAttribute(
      "src",
      "https://s3-us-west-2.amazonaws.com/s.cdpn.io/316871/termynal.min.js"
    );
    termynalScript.setAttribute("data-termynal-container", "#termynal");
    document.head.appendChild(termynalScript);
  }
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  align-content: center;
  font-size: 2em;
  color: black;
  margin: 0;
}

.main-text {
  margin: 40px;
}

.body-text {
  margin-top: 40px;
  margin-bottom: 80px;
}

.terminal {
  display: flex;
  justify-content: center;
}
</style>


