<template>
  <section>
    <h2>Hey there!</h2>
    <h1>My name is {{ name }}</h1>
    <h3 id="title">{{ title }}</h3>
  </section>
</template>

<script>
export default {
  data() {
    return {
      name: 'Uchenna',
      title: 'Software Engineer | Web Developer'
    };
  }
};
</script>
