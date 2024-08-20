<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Visit these links to view my
      <a href="https://www.linkedin.com/in/alex-mohamed-16352b290" target="_blank" rel="noopener">LinkedIn</a> and
      <a href="https://github.com/Alex-Mohamed" target="_blank" rel="noopener">GitHub</a>!
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

a:link,
a:active {
  color: blue;
}

a:visited {
  color:blueviolet;
}

.greetings h1 {
  text-align: center;
  color: aqua;
}

.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
}
  
</style>
