<template>
  <section>
    <!-- <h2>Hey there!</h2> -->
    <h2>My name is</h2>
    <!-- <h3 id="title">{{ title }}</h3> -->
  </section>
</template>

<script>
/* eslint-disable */
export default {
  data() {
    return {
      name: 'Uchenna',
      title: 'Software Engineer | Web Developer',
    };
  },
};
</script>

<style lang="scss" scoped>
@import '@/assets/mixins.scss';

section {
  width: 100%;
  height: 60vw;
  overflow: hidden;
  background: -moz-radial-gradient(
      center,
      ellipse cover,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url('/UchennaLinkedInHeader.png') no-repeat center center; /* FF3.6-15 */
  background: -webkit-radial-gradient(
      center,
      ellipse cover,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url('/UchennaLinkedInHeader.png') no-repeat center center; /* Chrome10-25,Safari5.1-6 */
  background: radial-gradient(
      ellipse at center,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url('/UchennaLinkedInHeader.png') no-repeat center center; /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  background-size: cover;
  color: #333;

  h1 {
    color: #63f105;
    margin-top: 0.95em;
    @include fluid-type(font-size, 320px, 1366px, 30px, 100px);
  }
  h2 {
    color: #63f105;
    margin-top: 0;
    padding-top: 1em;
    @include fluid-type(font-size, 320px, 1366px, 15px, 60px);
  }
  #title {
    color: orange;
    padding-top: 1.5em;
    @include fluid-type(font-size, 320px, 1366px, 15px, 50px);
  }
}
</style>
